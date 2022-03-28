---
layout: post
title:  "Windows中出现 Fatal Error C1060"
date:   2022-03-28 4:20:39
categories: Windows
---

## 32位Windows系统的内存2G限制会造成这个问题
### 可以使用3G开关获得更大内存:
### win 7 下：
```
打开3GB切换：
 - 在“开始”菜单下的“附件”程序组中，右击“命令提示器”（Command Prompt）。 点击“使用系统管理员身份运行”（Run as Administrator）。
 - 在命令提示器中输入“bcdedit /set IncreaseUserVa 3072”
 - 重启电脑。
```
```
关闭3GB切换：
 - 在“开始”菜单下的“附件”程序组中，右击“命令提示器”。 点击“使用系统管理员身份运行”。
 - 在命令提示器中输入“bcdedit /deletevalue IncreaseUserVa”
 - 重启电脑。
```

Created by Mo Yao