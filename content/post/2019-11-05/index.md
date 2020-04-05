+++
title =  "Retrieving a certificate and private key from a P12 file"
url = "2019-11-05"
date = "2019-11-05"
description = "Retrieving a certificate and private key from a P12 file"
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

How to retrieve a certificate and private key from a .p12 file.  
I needed it when I was writing AWS SNS with Terraform.  

{{< highlight html >}}
$ openssl pkcs12 -in xxxx.p12 -nodes -nokeys -out certificate.pem
$ openssl pkcs12 -in xxxx.p12 -nodes -nocerts -out privatekey.oem
{{< /highlight >}}


<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}


This way, however, the file will have text starting with NoArgument at the beginning.  
NoArgument doesn't do any harm when it's in, but I was curious about it, so I tried to remove it.
The secret key was converted without NoArgument by executing the following command.  
I gave up on the certificate because I couldn't find a way to erase the text.  
I'll post it if I can.

{{< highlight html >}}
$ openssl pkcs12 -in xxxx.p12 -nodes -nocerts | openssl rsa -out privatekey.pem
{{< /highlight >}}


参考: [Push通知の証明書、p12 -> pem変換について](http://ryokwkm2.hatenadiary.jp/entry/2016/08/10/095840)
