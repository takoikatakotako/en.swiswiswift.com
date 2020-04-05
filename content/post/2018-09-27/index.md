+++
title = "Build input file cannot be found: Libraries/WebSocket/libfishhook.a’"
url = "2018-09-27"
date = "2018-09-27"
description = "Build input file cannot be found: Libraries/WebSocket/libfishhook.a’"
tags = [
    "ReactNative",
]
categories = [
    "ReactNative",
]
archives = "2018/09"
aliases = ["migrate-from-jekyl"]
+++

<br>

Reference: 
[Xcode 10 libfishhook.a cannot be found](https://github.com/facebook/react-native/issues/19569)

When I updated Xcode to 10.0, I got the above error and couldn't compile ReactNative.

RTCWebSocket.xcodeproject -> RCTWebSocket -> Select Build Phases -> Add libfishhook.a to Link Binary WithLibraried.  
Delete if already added.  

The problem was solved by doing

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
