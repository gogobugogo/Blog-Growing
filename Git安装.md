---
title: Git - Mac安装指南
date: 2017-12-25
categories: 工具
tags: [Git]
---





Git是开源的分布式版本控制系统，这次搭建博客在Mac安装了Git，记录一下安装过程。

#### 下载Git

[Git官网][https://git-scm.com/downloads] 下载Mac版本的GIt安装包

双击.pkg安装



<!-- more -->



#### 检查是否安装成功

打开terminal，输入git \-\-version/which git，检查安装版本/路径



#### 创建用户

git config \-\-global user.name *your name*    //用户名

git config \-\-global user.email *your email*    //用户邮箱



#### 连接GitHub

[1] 进入根目录

[2] 输入ssh-keygen，生成ssh-key

[3] ～/.ssh/id_rsa.pub文件内容copy到GitHub -> Account -> Settings -> SSH and GPG keys -> new SSH key -> save



#### Git命令补全

[1] 下载[git-completion.bash][https://github.com/markgandolfo/git-bash-completion]

[2] 下载的git-bash-completion文件夹中，git-completion.bash放入～/目录（当前用户主目录）

[3] 重命名为.git-bash-completion：mv git-bash-completion .git-bash-completion

[4] 每次开启终端，执行此脚本：source .git-bash-completion

即可实现git命令自动补全



**参考文献**

\[1][Mac OS Git安装][https://www.cnblogs.com/chenlogin/p/5124318.html]