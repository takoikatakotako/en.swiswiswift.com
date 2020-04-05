+++
title = "Removing the back button in UINavigationController."
url = "2017-10-14"
date = "2017-10-14"
description = "Removing the back button in UINavigationController."
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2017/10"
aliases = ["migrate-from-jekyl"]
+++

<br>

Removes the text of the back button in UINavigationController.  
Change "< back" to "<".  

```
let backButton = UIBarButtonItem(title: "", style: .plain, target: nil, action: nil)
self.navigationItem.backBarButtonItem = backButton
self.navigationController?.pushViewController(picDetailView, animated: true)
```

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
