---
title: gitnote
cdn: 'header-off'
header-img: "http://wx1.sinaimg.cn/large/7decfc68gy1fosugpt7r0j20hs08c74n.jpg"
tag: git
---

## 术语

* HEAD: 指针指向当前分支
* master 主干分支

## 命令行

### 基本操作

* `git checkout --filename` 从当前版本恢复文件
* `git remove filename` 从当前版本库删除文件

### 分支操作

* `git checkout -b <name>` checkout后面加上参数`-b`,表示创建并切换
* `git branch` 查看所有分支，当前分支前会有`*`号
* `git checkout <name>` 切换分支
* `git branch <name>` 创建分支
* `git merge <name>` 当前分支与某分支合并
* `git branch -d <name>` 删除分支 

### cherry-pick操作
* `git cherry-pick <HashA> <HashB>`
* `git cherry-pick <HashA>..<HashB>`，选择A-B之间的系列提交，不包含A
* `git cherry-pick <HashA>^..<HashB>`，选择A-B之间的系列提交，包含A
* `git cherry-pick --continue` 冲突时，解决冲突后继续.

