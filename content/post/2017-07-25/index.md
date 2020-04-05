+++
title = "Sending JSON in post with curl"
url = "2017-07-25"
date = "2017-07-25"
description = "Sending JSON in post with curl"
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

How to post json from Mac terminal with curl command.  
I often use it when I'm developing locally and want to check the APIs.  

```
curl http://localhost:3000/api/url -X POST -H "Content-Type: application/json" -d '{"email":"kabigon@swiswiswift.com", "password":"password"}'
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
