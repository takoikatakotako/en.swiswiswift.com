+++
title =  "Displaying a Firestore image in SwiftUI"
url = "2020-02-08"
date = "2020-02-08"
description = "Displaying a Firestore image in SwiftUI"
tags = [
    "Swift", "SwiftUI", "Firebase"
]
categories = [
    "Swift", "SwiftUI", "Firebase"
]
archives = "2020/02"
aliases = ["migrate-from-jekyl"]
+++

<br>

How to display a Firestore image in SwiftUI.
UIImage can be easily displayed using SDWebImage, but SwiftUI can't do that.
I used [SDWebImage/SDWebImageSwiftUI](https://github.com/SDWebImage/SDWebImageSwiftUI) to write the following
I feel like there's a better way to write this, so that it's cached, including the tokens.

Reference:
[iOS でファイルをダウンロードする](https://firebase.google.com/docs/storage/ios/download-files?hl=ja)
[SDWebImage/SDWebImageSwiftUI](https://github.com/SDWebImage/SDWebImageSwiftUI)


<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako 255a693ee8426fa4fe1c24830be40935 >}}
