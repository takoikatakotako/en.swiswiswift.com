+++
title = "Docker image that can be SSHed in(CentOS7)"
url = "2018-12-25"
date = "2018-12-25"
description = "Docker image that can be SSHed in(CentOS7)"
tags = [
  "Docker",
]
categories = [
    "Docker",
]
archives = "2018/12"
aliases = ["migrate-from-jekyl"]
+++

<br>

For Ansible practice, I wrote this because I wanted an image that can be entered by SSH.

```
docker build -t ssh_centos7:latest . --no-cache
docker run -d -p 2222:22 ssh_centos7:latest
ssh-keygen -R [localhost]:2222
ssh -p 2222 kabigon@localhost
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako d3f4096b9301a56e05e7ab8239439fe6 >}}
