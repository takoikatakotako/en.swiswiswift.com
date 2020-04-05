+++
title = "Adopting UITest with Swift(Swift4.2)"
url = "2019-01-26"
date = "2019-01-26"
description = "Adopting UITest with Swift(Swift4.2)"
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2019/01"
aliases = ["migrate-from-jekyl"]
+++

<br>

Add the UITest to your project.  
If you didn't create it when you created the project, you can add it by following the steps in the image below.

Write `@testable import Swiswiswift` (Swiswiswift is the name of the project) so that you can refer to it in the test class.  
By prefixing the function name with "test", it can be executed as a test.

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako 026e20c64d4aa955e079024a7ea9340a >}}
