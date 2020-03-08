+++
title =  "Do not change the color of the Image in the Button with SwiftUI"
url = "2020-02-24"
date = "2020-02-24"
description = "Do not change the color of the Image in the Button with SwiftUI"
tags = [
    "Swift"
]
categories = [
    "Swift"
]
archives = "2020/02"
aliases = ["migrate-from-jekyl"]
+++

<br>

It is a way to do not change the color of the Image in the Button with SwiftUI.
If you keep the default, the color will change to blue as in the following image.

![ButtonColor](1.png)

By setting `renderingMode(.original)` the color of the original image was displayed.

![ButtonColor](2.png)

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako 5f965173af83b27d15e60f65ef0031a5 >}}
