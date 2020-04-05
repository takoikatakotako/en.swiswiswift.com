+++
title = "I also want to check the response header when sending JSON in post with curl"
url = "2017-07-26"
date = "2017-07-26"
description = "I also want to check the response header when sending JSON in post with curl"
tags = [
    "Linux",
]
categories = [
    "Linux",
]
archives = "2017/07"
aliases = ["migrate-from-jekyl"]
+++

<br>

I used it when I wanted to check the response header when sending JSON in post with curl.
If you add `--include` at the end, the response header is also shown.

```
http://localhost:3000/api/url -X POST -H "Content-Type: application/json" -d '{"email":"user@swiswiswift.com", "password":"password"}'--include
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
