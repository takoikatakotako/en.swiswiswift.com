+++
title = "UIBarButtonItem"
url = "2017-05-04"
date = "2017-05-04"
description = "UIBarButtonItem"
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2017/05"
aliases = ["migrate-from-jekyl"]
+++

<br>

UIBarButtonItem used to add or customize elements in UINavigationBar.

Class hierarchy of UIBarButtonItem

NSObject  
↑  
UIBarItem  
↑  
UIBarButtonItem  
[AppleDeveloperリファレンスUIBarButtonItem](https://developer.apple.com/documentation/uikit/uibarbuttonitem)

UIBarButtonItem example sentence

Generate a UINavigationBar and put a title and button on it.

![alt](1.png)

{{< gist takoikatakotako 401a75d396db4548302b32e757f44e52 >}}


Changing the color of UIBarButtonItem

UIBarButtonItem is blue by default, but the color can be specified in the following way.  
Change color of Back button in navigation bar

```
//ナビゲーションボタンの色を変更する
UINavigationBar.appearance().tintColor = UIColor.black
UIBarButtonSystemItem
```

UIBarButtonSystemItemを用いることで、デフォルトに入っているボタンを使用することができます。  
https://developer.apple.com/reference/uikit/uibarbuttonsystemitem

```
//barButtonSystemItem:に  [.add]を設定することで[+]ボタンを設定する,上のコード参照
let leftNavBtn =  UIBarButtonItem(barButtonSystemItem:  .add, target: self, action: #selector(leftBarBtnClicked(sender:)))
```

- Add
- Done
- Cancel
- Edit
- Save
- Compose
- Reply
- Action
- Organize
- Bookmarks
- Search
- Refresh
- Stop
- Camera
- Trash
- Play
- Pause
- Rewind
- Undo
- Redo
- PageCurl

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
