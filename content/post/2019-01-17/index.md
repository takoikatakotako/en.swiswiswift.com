+++
title = "tar (child): gzip: Cannot exec: No such file or directory"
url = "2019-01-17"
date = "2019-01-17"
description = "tar (child): gzip: Cannot exec: No such file or directory"
tags = [
  "Linux",
]
categories = [
  "Linux",
]
archives = "2019/01"
aliases = ["migrate-from-jekyl"]
+++

<br>
The `tar` command was not able to solve the problem.

```
$ tar -zxvf openjdk-11.0.1_linux-x64_bin.tar.gz

tar (child): gzip: Cannot exec: No such file or directory
tar (child): Error is not recoverable: exiting now
tar: Child returned status 2
tar: Error is not recoverable: exiting now
```

The problem was solved by including the dependency package `gzip`.

```
$ yum install gzip
```
