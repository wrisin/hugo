---
title: "Hugo on Vercel 零基础"
date: 2020-08-07T00:48:47+08:00
draft: true
---

#### 一、注册Vercel并部署Hugo

1.到vercel官网注册一个号，然后点击右边select template；

2.选择Hugo；

3.选择personal account，然后继续；

4.按提示绑定github，然后继续（github注册过程略）；

5.点击Deploy，等待部署完成；

6.在菜单选择domains，选择Add，按提示添加域名。（没有域名此步省略）

#### 二、下载Github Desktop并克隆代码

可以使用Git等其他工具，此处只说Github Desktop；

1.下载登录Github Desktop，按提示操作；

2.从右列表选择刚才Vercel创建的项目进行克隆。

#### 三、在本机上安装Hugo

注意，此步不是为了将Hugo程序部署在电脑上，而是为了使用hugo的命令。Vercel目前我还没找到可以直接敲代码的方法，所以将Hugo安装在本地，这样就可以方便使用命令来操作我们克隆下来的程序。

原理：本地Hugo命令→克隆的Hugo→Github→Vercel

**以Windows为例**

1.安装chocolatey

管理员权限打开powershell，输入以下代码：

`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

回车等待安装完成；

2.安装Hugo

接着输入以下代码：

`choco install hugo -confirm`

回车等待安装完成。

#### 四、操作流程

**1.更换主题**

（1）点击github上的主题的绿色按钮code，选择open with github desktop；

（2）允许打开后，选择github desktop的克隆地址为克隆的Hugo程序的themes文件夹，点击克隆等待完成。

（3）删除刚下载的主题文件夹里的.git文件夹（是隐藏文件）；

（4）修改hugo根目录的config.toml，将themes名改为下载的主题的目录名。例如：`theme = "ananke" → theme = "contrast-hugo"`；

（5）回到github desktop，点击左下角commit to master（可能要填tag）；

（6）点击上方第二行栏目的push origin上传到github。

**2.生成文章**

（1）打开powershell，进入hugo程序目录。例如：`cd d:\hugo`；

（2）输入以下代码：`hugo new xxx/xxx.md` ，前处xxx代表文章分类目录，后处代表文章文件名，可以不是文章标题，直观显示在网址上，文章标题可以打开md文件修改；

（3）打开并修改md内容，图省事可以直接在---下方直接写正文。md编辑器推荐Typora；

（4）使用github desktop上传github。

（未完待续）



相关链接：

[Vercel](https://vercel.com/)

[Github Desktop](https://desktop.github.com/)

[Hugo官方文档-Install Hugo](https://gohugo.io/getting-started/installing/)

[Installing Chocolatey](https://chocolatey.org/install)

[Github代下载服务](http://g.widora.cn/)（github下载慢用这个）

[Hugo Themes](https://themes.gohugo.io/)