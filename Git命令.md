---
title: Git命令
date: 2018-05-24
categories: [工具]
tags: [Git]
---

#### 初始化

`git init`

#### 分支

[1] 查看本地分支

​      `git branch`

[2] 查看远端分支

​      `git branch -r`

[3] 查看所有分支

​      `git branch -a`

<!--more -->

[4] 本地创建新分支

​      `git branch [name]`

[5] 本地切换到新分支

​      `git checkout [name]`

[6] 本地创建&切换到新分支

​      `git checkout -b [name]`

[7] 新分支推送远端仓库

​      `git push origin [name]`

[8] 本地删除分支

​      `git branch -d [name]`

[9] 远端删除分支

​      `git push origin :[name]`