+++
title =  "Sending push notifications to your app with cURL (curl)"
url = "2019-11-06"
date = "2019-11-06"
description = "Sending push notifications to your app with cURL (curl)"
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2019/11"
aliases = ["migrate-from-jekyl"]
+++

<br>

How to send push notifications to iOS devices with the curl command.

Create a PEM file that includes both the certificate and the private key.


{{< highlight html >}}
$ openssl pkcs12 -in xxxx.p12 -nodes -out certificate-and-privatekey.pem
{{< /highlight >}}

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

The `curl` command is used to send a push notification.  
Push payloads, topics, and debit tokens should be from your environment.  
Also, be aware that the domain (https://api.push.apple.com/3/device/ or https://api.development.push.apple.com) is different between the production environment (e.g. test flights) and the development environment.  


{{< highlight html >}}
# Production Server
$ curl -v -d '{"aps":{"alert":"hello"}}' -H "apns-topic: com.swiswiswift.myapp" --http2 --cert certificate-and-privatekey.pem https://api.push.apple.com/3/device/{your_device_token}
# Staging Server
$ curl -v -d '{"aps":{"alert":"hello"}}' -H "apns-topic: com.swiswiswift.myapp" --http2 --cert certificate-and-privatekey.pem https://api.development.push.apple.com/3/device/{your_device_token}
{{< /highlight >}}
