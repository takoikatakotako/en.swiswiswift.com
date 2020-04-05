+++
title =  "Getting into an Alpine based container with Docker"
url = "2019-12-21"
date = "2019-12-21"
description = "Getting into an Alpine based container with Docker"
tags = [
    "Docker"
]
categories = [
    "Docker"
]
archives = "2019/12"
aliases = ["migrate-from-jekyl"]
+++

<br>

There are times when you want to go inside a Docker container and use a shell.
Normally, you would use the following command to enter the container, but on the Alpine base, you would use ash instead of bash to enter the container.

```
$ docker run --rm -t -i centos:centos7 /bin/bash
```
s

```
$ docker run --rm -t -i alpine:latest /bin/ash
```

参考  
[Dockerコンテナのシェルの中に入る](https://qiita.com/__cooper/items/4740c24666299c366044)
[dockerでalpine linux ベースのcontainerに入って、shellを使いたいとき。](https://qiita.com/yutachaos/items/56dd7ea09d7e2b0d9173)


<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
