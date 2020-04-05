+++
title = "Docker image that can be SSHed in(CentOS6)"
url = "2018-11-19"
date = "2018-11-19"
description = "Docker image that can be SSHed in(CentOS6)"
tags = [
    "Docker",
]
categories = [
    "Docker",
]
archives = "2018/11"
aliases = ["migrate-from-jekyl"]
+++

<br>

For Ansible practice, I wrote this because I wanted an image that can be entered by SSH.

```
$ docker build -t docker_ssh:latest .
$ docker run -d -p 2222:22 docker_ssh:latest
$ ssh -p 2222 kabigon@localhost
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako 14d4ebc02fb6d19e6b20999226534c44 >}}
