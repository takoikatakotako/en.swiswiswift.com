+++
title = "I sent a code-level question to an Apple engineer."
url = "2018-05-21"
date = "2018-05-21"
description = "I sent a code-level question to an Apple engineer."
tags = [
    "iOS",
]
categories = [
    "iOS",
]
archives = "2018/05"
aliases = ["migrate-from-jekyl"]
+++

<br>

My friends often tell me that AppleDeveloper registration fees are too high, but there are many good things in spite of the high fees.  
One of them is Technical Support Incident (TSI), where Apple engineers can answer questions and consult with you at the code level about bugs or problems that cannot be fixed.  
Register or update your AppleDeveloperProgram to receive two technical support rights.  

I've made an alarm clock app before, and there was a bug in the process that I couldn't resolve.  
Specifically, it's "Notification sound doesn't sound while iPhone is locked", and although it works in simulator, the bug appears in real machine.  
I couldn't solve it myself, so I decided to use DTI.  

First, I created an Xcode project with the buggy part cut out and put it up on github.  
Next, I wrote the "Title", "Bug Description", "Reproduction Instructions", and "App Name and App ID" in English, and sent it through the Code-Level Support form on my account page (https://developer.apple.com/account/?view=support).  
I received an auto-response email immediately, so I attached an Xcode project (the same one I put up on github) with the part of the bug I cut out to the email and replied.  

Two days later, I received a reply from an Apple engineer.  
Thanks for the Xcode project and reproducibility instructions! I followed your instructions and didn't get any bugs in my environment. My wife and I borrowed a friend's terminal and it worked fine.  
My iPhone seems to have been broken. orz.  

It's a boring ending, but I really appreciated having an Apple engineer actually work with the code and try it out, and I was grateful when I got really stuck.  

Have a great Swift life!  

AppleDeveloper - Technical Support Requests  
https://developer.apple.com/jp/support/technical/  

<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}
