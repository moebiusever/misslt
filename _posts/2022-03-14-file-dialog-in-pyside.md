---
layout: post
title:  "PySide中的文件对话框!"
date:   2016-06-04 13:50:39
categories: jekyll
---

## 文件保存对话框
PySide:

```
fileName = QFileDialog.getSaveFileName(self, self.tr("Export"), "", \
    self.tr("Data Files (*.csv)"))
print(fileName)
with open(fileName[0], "wb") as f:
    f.write("test")
```

## 文件打开对话框
PySide:

```
fileName = QFileDialog.getOpenFileName(self, self.tr("Export"), "", \
    self.tr("Data Files (*.csv)"))
print(fileName)
with open(fileName[0], "rb") as f:
        f.read(）
```

Created by Mo Yao