---
layout: post
title:  "查看glibc的版本和兼容性"
date:   2022-04-06 15:15:39
categories: Linux
---

## 其他发行版

```
strings /lib64/libc.so.6 | grep GLIBC
strings /lib/libc.so.6 | grep GLIBC
```

## deepin 20.04

```
strings /usr/lib/x86_64-linux-gnu/libc.so.6 | grep GLIBC
strings /usr/lib/i386-linux-gnu/libc.so.6 | grep GLIBC
```

Created by Mo Yao