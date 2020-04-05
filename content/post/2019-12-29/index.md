+++
title =  "Remove Storyboards from projects running iOS13 and above"
url = "2019-12-29"
date = "2019-12-29"
description = "Remove Storyboards from projects running iOS13 and above"
tags = [
    "Swift", "iOS"
]
categories = [
    "Swift", "iOS"
]
archives = "2019/12"
aliases = ["migrate-from-jekyl"]
+++

<br>

Create a file with `Swift` & `Storyboard`.
Removes `Main.storyboard`.

![Delete Storyboard](1.png)

Delete the term `Main storyboard file base name`.

![Delete Main In Info.plist](2.png)

`Application Scene Manifest` -> `Application Session Role` -> `Item0` -> Remove the `Storyboard Name`.

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}


![Delete Storyboard Name](3.png)

Set the ViewController to be displayed with `SceneDelegate.swift`.

```
func scene(_ scene: UIScene, willConnectTo session: UISceneSession, options connectionOptions: UIScene.ConnectionOptions) {
    guard let windowScene = (scene as? UIWindowScene) else { return }
    window = UIWindow(frame: UIScreen.main.bounds)
    let viewController = ViewController()
    window?.rootViewController = viewController
    window?.makeKeyAndVisible()
    window?.windowScene = windowScene
}
```

参考  
[Creating Apps Without Storyboards in iOS 13](https://medium.com/better-programming/creating-apps-without-storyboards-in-ios-13-fc9550bb9c12)
