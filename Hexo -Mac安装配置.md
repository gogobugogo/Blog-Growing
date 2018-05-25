---
title: Hexo - Mac安装配置
date: 2017-12-30
categories: 工具
tags: [Blog]
---

 心血来潮想要写博客，记录、总结一下自己学习过程中遇到的问题，也方便自己后面查阅和复习。现在流行的一些博客网站不够简洁，广告也多，最终决定用Hexo + 模板搭建个人博客，部署在Github。

#### 安装Node.js

[Node.js官网][https://nodejs.org/en/]下载安装最新版本的Node.js。

下载pkg版本，直接点击安装。安装完成后，在terminal中输入`npm -v`和`node -v`，出现版本信息说明安装成功。

<!-- more -->

#### 安装Git

[Git官网][https://git-scm.com/download/mac]下载安装最新版本的Git。

安装步骤参考[Git安装指南][https://gogobugogo.github.io/2017/12/25/Git安装/]。

#### 安装Hexo

Node.js和Git安装完成后，执行以下命令安装Hexo：

`sudo npm install -g hexo`

创建文件夹hexo，cd到hexo中执行命令`hexo init`完成安装、初始化。

#### 配置Hexo

修改_config.yml的配置信息。

e.g.  title：Blog名称

​        author：作者名

​        language：zh-Hans（中文简体）

与user_name.github.io建立关联，需要配置：

> deploy:
>
> ​	type: git
>
> ​	repository: git@github.com:user_name/user_name.github.io.git

#### 发布文章

利用命令`hexo generate`生成静态页面。`hexo server`命令启动本地服务，可在http://localhost:4000查看。`hexo deploy`命令发布博客，可在http://user_name.github.io 查看。

每次发布博客，依次执行命令：

`hexo clean`

`hexo generate`

`hexo deploy`

即可。

#### 博客主题

下载[Next主题][https://github.com/iissnan/hexo-theme-next]放置到hexo/themes。修改配置_config.yml：

> theme： next

重新发布后，博客即使用Next主题。

#### 博客文章

使用Markdown编写的博客文章放在hexo/source/_posts目录下。文章开头指定文章标题、日期、分类和标签。

> title: Hexo - Mac安装配置
> date: 2018-12-30
> categories: 工具
> tags: [Blog]

至此，已经完成博客基本功能的配置。

利用Hexo搭建个人博客，优点是可以自由更换主题、没有广告、命令简单，希望我可以坚持写下去，探索更多的功能。