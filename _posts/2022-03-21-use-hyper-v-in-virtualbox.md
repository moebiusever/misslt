---
layout: post
title:  "在Virtualbox中使用Hyper-V"
date:   2022-03-16 13:50:39
categories: Virtualbox
---

## 配置VirtualBox

VirtualBox 只有 6.0 以上的版本才能兼容 Hyper-V. 最好在一个全新的环境下操作。

找到 VirtualBox 的安装目录，在那里用 powershell 执行以下命令：

```
#对所有虚拟系统启用Hyper-V支持
./VBoxManage.exe setextradata global "VBoxInternal/NEM/UseRing0Runloop" 0
```
```
#只对某特定系统启用Hyper-V支持
./VBoxManage.exe setextradata "<虚拟机名字>" "VBoxInternal/NEM/UseRing0Runloop" 0
```

Created by Mo Yao