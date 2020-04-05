+++
title = "Selecting an image with ImagePickerController(Swift4.2)"
url = "2019-01-11"
date = "2019-01-11"
description = "Selecting an image with ImagePickerController(Swift4.2)"
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

`# Swift 4.2`

Read the Swift3 article here.  
Selecting images with UIImagePickerController

It is a sample program to get an image from the photo library of the iPhone.  
In order to select images from the photo library, the project's info.plist should state that the photo library will be used.  
If you don't write this, UIImagePickerController won't work.  
Use the following values for the key  
`NSPHOtoLibraryUsageDescription`.
The Type is a String and the reason for use is written in the Value.  
I've heard that if you don't write the reason for using it, it will be rejected at the time of examination.  

![alt](1.gif)

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako a73bf357ab9fe77db1a81c08dc4b62ef >}}
