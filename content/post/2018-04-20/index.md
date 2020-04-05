+++
title = "Get the current date and day of the week and the current time"
url = "2018-04-20"
date = "2018-04-20"
description = "Get the current date and day of the week and the current time"
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2018/04"
aliases = ["migrate-from-jekyl"]
+++

<br>

Sample code to get the current date, day of the week, and current time in Swift4.1.  
You can get it as a string of the following format.  

Thu, Apr 03, 2018  
19:03:34  

Here is the sample code to get it in the form shown above.  

If you use Calendar.current, there is a possibility that you will get it in Japanese calendar (Heisei 00 year) depending on the setting (you want 2018/04/03, but 30/04/03 comes back), so it is better to get it in Gregorian calendar.  
On the other hand, if you want a Japanese calendar, there is a way to get a Japanese calendar.

This site is detailed.  
[Swift 3 の日時操作チートシート](https://qiita.com/mishimay/items/8d67b583dc6809b2baf5)  

Other sites that I found helpful  
[Swift3での日時に関する処理](https://qiita.com/isom0242/items/e83ab77a3f56f66edd2f)  
[【Swift3】現在時刻の取得とDataFormatterでの文字列化](https://qiita.com/GDaigo/items/270e6ed6e898e8b8e1c3)  

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}

{{< gist takoikatakotako 9f029788e0b3ea4985719a87d657614b >}}
