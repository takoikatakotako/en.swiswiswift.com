+++
title =  "Use Docker to set up PostgreSQL and create tables."
url = "2019-11-22"
date = "2019-11-22"
description = "Use Docker to set up PostgreSQL and create tables."
tags = [
    "Docker"
]
categories = [
    "Docker"
]
archives = "2019/11"
aliases = ["migrate-from-jekyl"]
+++

<br>
This is how to build a PostgreSQL using Docker.  
It's great to maintain your development environment with Docker because you don't have to pollute your local environment.

[postgres-Docker Hub](https://hub.docker.com/_/postgres)

The following command allows you to set up postgres11 on the local 5432 port and log in as a user named kabigon. (password is password)  
A database called pokemon is also created at the same time.

```
$ docker run -d -p 5432:5432 -e POSTGRES_USER=kabigon -e POSTGRES_PASSWORD=password -e POSTGRES_DB=pokemon postgres:11
$ psql -h localhost -p 5432 -U kabigon -d pokemon
```

After login, show the list of databases with the `\\*l command, and make sure that the pokemon database is displayed.

Also, if you put `.sql` in `docker-entrypoint-initdb.d`, it will be executed at initialization.
This is useful when you want to create an initial table, etc.  
If you create `setup.sql` in the `initdb` directory and mount the directory, `.sql` will be executed when the container is initialized.

```setup.sql
create table pokemon
(
  id int8,
  name varchar
);

create table pokemon_gym
(
  id int8,
  area varchar
);
```

```
$ docker run -v $PWD/initdb:/docker-entrypoint-initdb.d -d -p 5432:5432 -e POSTGRES_USER=kabigon -e POSTGRES_PASSWORD=password -e POSTGRES_DB=pokemon postgres:11
$ psql -h localhost -p 5432 -U kabigon -d pokemon
```

```
pokemon=# \d
List of relations
 Schema |    Name     | Type  |  Owner  
--------+-------------+-------+---------
 public | pokemon     | table | kabigon
 public | pokemon_gym | table | kabigon
```

We have confirmed that the `pokemon` and `pokemon_gym` tables have been created.

If it doesn't work well, you may want to go into the container and check if there is a `.sql` in the `docker-entrypoint-initdb.d`.


```
$ docker ps
$ docker exec -it 9dfa9b7caa7f bash
```

### おまけ

This is the case when you use docker-compose.

```
version: '3'

services:
  postgres:
      container_name: my-postgres
      image: postgres:11
      ports:
        - "5432:5432"
      environment:
        - POSTGRES_USER=dev
        - POSTGRES_PASSWORD=password
        - POSTGRES_DB=dev
      volumes:
        - ./postgres/initdb:/docker-entrypoint-initdb.d
```


```
.
├── docker-compose.yaml
└── postgres
    └── initdb
        └── setup.sql
```

```
$ docker-compose up -d --force-recreate
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
