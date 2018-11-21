# wllyy189.github.io

Myblog -> http://www.wangle.pub

## 简介

本教程记录如何在`GitHub`上搭建博客。从中可以掌握部分`GitHub Pages`功能，`Jekyll`软件的基本用法，以及`Disqus`评论系统的基本用法。

### GitHub Pages
[GitHub](https://github.com) 是通过`Git`进行版本控制的软件源代码托管服务，允许个人用户创建公开的代码仓库。号称程序员界的 `Facebook`，事实上它已成为了世界上最大的代码存放网站和开源社区。
`GitHub`设计了 [GitHub Pages](https://pages.github.com) 功能允许用户为自己的项目提供网页展示，来替代默认的代码列表。`GitHub Pages`可以被认为是用户编写的，托管在 github 上的静态网页。

### Jekyll
[Jekyll](https://jekyllrb.com) （发音/'dʒiːk əl/，“杰克尔”）是一个静态网页的生成工具，不需要数据库支持。可以免费部署在`GitHub`上，而且可以绑定自己的域名。

### Disqus
[Disqus](https://disqus.com) 是一家第三方社会化评论系统，主要为网站提供评论托管服务。

## 快速入门

### 注册 GitHub 账号

要使用`GitHub Pages`服务，首先要注册一个 [GitHub](https://github.com) 账号。

### 创建一个项目

### 安装Jekyll

[Jekyll 中文文档](http://jekyll.com.cn)，英语水平一般的福利。
我的办公环境是 Windows 系统，所以下面我讲述的是`Jekyll`在 Windows 下的安装指南。

**安装Ruby**

- 下载 [Ruby](http://rubyinstaller.org/downloads) 安装包，建议下载`Ruby+Devkit`，根据你的系统版本进行选择，我是64位操作系统，所以选择 x64 版本。
- 下载后双击`rubyinstaller-devkit-x.x.x.x-x64.exe`进行安装，安装最后一步选择继续安装`MSYS2`，最后选择输入3（msys2 and mingw development toolchain）。

**使用命令行安装Jekyll**
```
gem install jekyll
```
所有`Jekyll`的依赖包都会被自动安装