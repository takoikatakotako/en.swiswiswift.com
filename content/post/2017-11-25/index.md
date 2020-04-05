+++
title = "Removing @objc inference warnings when migrating from Swift3 to Swift4"
url = "2017-11-25"
date = "2017-11-25"
description = "Removing @objc inference warnings when migrating from Swift3 to Swift4"
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2017/11"
aliases = ["migrate-from-jekyl"]
+++

<br>

When I switch from Xcode8 to Xcode9 and convert to Swift4, I get the following error. Here's how to make it disappear.  

```
The use of Swift 3 @objc inference in Swift 4 mode is deprecated. Please address deprecated @objc inference warnings, test your code with “Use of deprecated Swift 3 @objc inference” logging enabled, and then disable inference by changing the "Swift 3 @objc Inference" build setting to "Default" for the "TargetName" target.
```

Select each target -> Build Settings -> Search for inference in the search window -> Set Swift @objc inference to Default　  
If there are other targets (UITest and UnitTest), set them to Default too.  
It should be gone now!  

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
