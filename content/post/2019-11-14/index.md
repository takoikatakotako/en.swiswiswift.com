+++
title =  "SwiftUI gets used a lot with Struct"
url = "2019-11-14"
date = "2019-11-14"
description = "SwiftUI gets used a lot with Struct"
tags = [
    "iOS", "Swift"
]
categories = [
    "iOS", "Swift"
]
archives = "2019/11"
aliases = ["migrate-from-jekyl"]
+++

<br>
I wanted to display a different ID for each screen transition, but I couldn't do that. (The same ID is displayed each time.)

![SameID](1.gif)

This was avoided by regenerating the id with `onDisappear`.  
If there is no change in `@State`, does that mean that you use the cache?   
I'm going to learn more about it!

![SameID](2.gif)

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako 8fa1b637dcc404f99c78f4c2af84c2a4 >}}
