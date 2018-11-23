---
layout: post
title: "GitHub Pages博客全教程"
subtitle: " \"GitHub Pages Blog\""
date: 2018-11-22 15:00:00
author: "王樂"
header-img: "assets/20181122/post-bg-20181005.jpg"
catalog: true
tags:
    - 笔记
---

> “Happy Birthday.”


## 前言

2018年国庆从贵州旅行回到深圳，一直想有个地方可以写点东西。

于是乎翻出注册已久的域名 wangle.pub 开始折腾，花了一天时间终于 [LeW Blog](https://wangle.pub) 开通了。

搭建博客我主要选择的 [GitHub Pages](https://pages.github.com/) + [Jekyll](https://jekyllrb.com/) 技术方案。

原因如下：

- **Markdown** — 已融入到程序生涯中，具备优雅的写作体验。
- **免费** — 利用 GitHub Pages 的域名和免费无限空间，不用自己采购云主机。
- **Git工作流** — 非常熟悉的程序流程，Git Commit + Push 即可发布博文。


## 简介

本教程记录如何在`GitHub`上搭建博客。从中可以掌握部分`GitHub Pages`功能，`Jekyll`软件的基本用法，以及`Disqus`评论系统的基本用法。

### GitHub Pages
[GitHub](https://github.com) 是通过`Git`进行版本控制的软件源代码托管服务，允许个人用户创建公开的代码仓库。号称程序员界的 Facebook，事实上它已成为了世界上最大的代码存放网站和开源社区。
GitHub 设计了 [GitHub Pages](https://pages.github.com) 功能允许用户为自己的项目提供网页展示，来替代默认的代码列表。GitHub Pages 可以被认为是用户编写的，托管在 GitHub 上的静态网页。

### Jekyll
[Jekyll](https://jekyllrb.com) （发音/'dʒiːk əl/，“杰克尔”）是一个静态网页的生成工具，不需要数据库支持。可以免费部署在 GitHub 上，而且可以绑定自己的域名。

### Disqus
[Disqus](https://disqus.com) 是一家第三方社会化评论系统，主要为网站提供评论托管服务。


## 开始搭建

### 安装Jekyll

[Jekyll 中文文档](http://jekyll.com.cn)，英语水平一般的福利。
我的办公环境是 Windows 系统，所以下面我讲述的是 Jekyll 在 Windows 下的安装指南。

**安装Ruby**

- 下载 [Ruby](http://rubyinstaller.org/downloads) 安装包，建议下载`Ruby+Devkit`，根据你的系统版本进行选择，我是64位操作系统，所以选择 x64 版本。
- 下载后双击`rubyinstaller-devkit-x.x.x.x-x64.exe`进行安装，安装最后一步选择继续安装`MSYS2`，最后选择输入3（msys2 and mingw development toolchain）。

**使用命令行安装 Jekyll**
```
gem install jekyll
```
所有`Jekyll`的依赖包都会被自动安装。

###  注册 GitHub 账号

要使用 GitHub Pages 服务，首先要注册一个 [GitHub](https://github.com) 账号。

### 创建一个项目仓库

![](https://upload-images.jianshu.io/upload_images/1120919-3c06b2e6cc3415a7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

仓库名为`你的GitHub用户名.github.io`，例如：`wllyy189.github.io`

### 导入仓库模版

可下载该仓库 [startbootstrap-clean-blog-jekyll](https://github.com/BlackrockDigital/startbootstrap-clean-blog-jekyll) 代码，导入到刚刚创建的博客仓库中。感谢这个作者。

这时如果安装好了 Jekyll，只需要在该仓库目录下的命令行输入 `jekyll serve` 就能在本地浏览器预览主题。

### 注册 Disqus 帐号

为了给 Blog 加上评论系统，需要一个第三方的服务，可选择 [Disqus](https://disqus.com/)、[Duoshuo](http://duoshuo.com/)、[Gitalk](https://github.com/gitalk/gitalk)。我选择的是 Disqus。

注册好 Disqus 帐号后需要在账户下创建一个站点：

![](https://upload-images.jianshu.io/upload_images/1120919-c35e8fbe252e7059.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

配置个人信息：

![](https://upload-images.jianshu.io/upload_images/1120919-a4a4be960868b689.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

记录好`Shortname`：

![](https://upload-images.jianshu.io/upload_images/1120919-d4204512209a1760.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

配置授信域名：

![](https://upload-images.jianshu.io/upload_images/1120919-2dae1032ed133739.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

到此 Disqus 帐号及配置已基本准备完毕。


