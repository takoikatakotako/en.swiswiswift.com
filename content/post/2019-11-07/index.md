+++
title =  "Create a really simple mock server with PHP"
url = "2019-11-07"
date = "2019-11-07"
description = "Create a really simple mock server with PHP"
tags = [
    "PHP",
]
categories = [
    "PHP",
]
archives = "2019/11"
aliases = ["migrate-from-jekyl"]
+++

<br>

I needed a local mock server, so I made a simple one in PHP.  
Register a user at `signup.php`, show a list of users at `list.php`, and remove all users at `deleate.php`.

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< highlight html >}}
# Server Start
$ php -S localhost:8000
{{< /highlight >}}

{{< highlight html >}}
# Regist User
$ curl http://localhost:8000/signup.php -X POST -H "Content-Type: application/json" -d '{"name":"onojun", "age":24}'
{{< /highlight >}}

{{< highlight html >}}
# User List
$ curl http://localhost:8000/list.php
{{< /highlight >}}

{{< highlight html >}}
# Delete All User
$ curl http://localhost:8000/deleate.php
{{< /highlight >}}

{{< gist takoikatakotako 75bce07d6d7600a0b09b947bd45332ed >}}
