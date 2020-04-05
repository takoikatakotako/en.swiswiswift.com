+++
title =  "A summary of words I didn't know when I was an infrastructure engineer"
url = "2019-11-08"
date = "2019-11-08"
description = "A summary of words I didn't know when I was an infrastructure engineer"
tags = [
    "AWS",
]
categories = [
    "AWS",
]
archives = "2019/11"
aliases = ["migrate-from-jekyl"]
+++

<br>

I put together a list of words I looked up when I started studying infrastructure and didn't understand them.

### Consolidated Billing
A bulk billing feature, available in AWS Organizations, that allows you to collectively bill payer accounts for all charges on an organization's consolidated accounts. It will be possible to track the costs of consolidated accounts.

### Root Account
You can log in as the root account by signing in to the AWS Management Console with the email address and password you used to create your AWS account.
The root account will have full and unrestricted access to all the resources of the AWS account, and its access privileges cannot be restricted.
- I don't usually sign in with my root account.
- Do not use AWS account (root) access keys
- Enabling AWS Multi-Factor Authentication (MFA)

### IAM: Identity and Access Management
A web service to securely console access to AWS resources, using IAM to control users who are authenticated (signed in) and allowed (with permissions) to use the resource.

### IAM User
An IAM user is a person or service that uses an IAM user to operate AWS.
IAM users are primarily used when a user signs in to the AWS Management Console to perform an interactive task or when making a programmatic request for an AWS service using the API or CLI.
There are two types, one for GUI and the other for CLI.

### IAM Group
An IAM group is a collection of IAM users.
Groups can be used to specify access privileges for a set of users, making it easy to manage user access privileges.

### Policy
A policy is a document that registers the actions that a user can perform and the resources that the actions can affect.
IAM users can be grouped into IAM groups and policies can be attached to those groups. All users of the group have permissions as per the policy attached to the group.

### Region
A geographically remote area where physical servers are located. ap-northeast-1 is Japan. us-west-2 is Oregon.

### Availability Zone
The location of the data center, I heard a rumor that AP-NORTheast-1A is in Shinagawa and AP-NORTheast-1C is in Saitama.

### Rolling Deployment
How to deploy and release a new application to multiple running servers in a fixed number of days. There is In-Place Deployment and Immutable Deployment.

### In-Place Deployment
How to deploy and restart a new application directly against a running server.

### Immutable Deployment
Deploy and test the new application in a new environment separate from the running server, and if all is well, switch to the new environment and delete the old one. If you want to roll back, also release the old application to the new environment and switch.

### Blue/Green Deployment
Deploy a new application to a different server (green) than the running server (blue) and check its operation.

### Canary Deployment
How to deploy and release a new application on only a portion of a running server. New services can be validated by allowing only specific users to use the new application. A deployment method that focuses only on the number of deployments, no matter how you deploy it.



<!-- Google Ads -->
{{< google-ads >}}

<!-- Amazon Ads -->
{{< amazon-ads >}}


## 参考
[AWS ドキュメント](https://docs.aws.amazon.com/)  
[AWSを安全に利用するために - ルートアカウント利用禁止、IAMを使う](https://qiita.com/tonishy/items/9eb772b4a5a338ac6ee6#24-iam%E3%82%B0%E3%83%AB%E3%83%BC%E3%83%97)  
[クラウドインフラエンジニア採用のための面談時質問シート](https://qiita.com/raki/items/4347366f78b8580d9f54)  
[近年のデプロイ手法について](https://clonos.jp/knowledge/detail14/)  
