+++
title = "Get and display the class name, function name and line number in Swift"
url = "2017-06-15"
date = "2017-06-15"
description = "Get and display the class name, function name and line number in Swift"
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2017/06"
aliases = ["migrate-from-jekyl"]
+++

<br>

We can't move in here! The debugging will be quicker if you write it in a part of the  
The class name and line number, retrieved can be displayed.  

```
print("Class name : \(NSStringFromClass(type(of: self))) ")
print(#function, #line)
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
