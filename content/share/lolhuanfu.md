---
title: "【教程】利用英雄联盟东南亚服，实现几个服切换着玩"
date: 2014-01-24T00:00:00+08:00
lastmod: 2020-08-29T20:41:28+08:00
draft: true
#keywords: []
#description: ""
#tags: []
categories: [分享]
author: "AceDog"

# You can also close(false) or open(true) something for this content.
# P.S. comment can only be closed
comment: false
toc: false
autoCollapseToc: false
postMetaInFooter: false
hiddenFromHomePage: false
# You can also define another contentCopyright. e.g. contentCopyright: "This is another copyright."
contentCopyright: false
reward: false
mathjax: false
mathjaxEnableSingleDollar: false
mathjaxEnableAutoNumber: false

# You unlisted posts you might want not want the header or footer to show
hideHeaderAndFooter: false

# You can enable or disable out-of-date content warning for individual post.
# Comment this out to use the global config.
#enableOutdatedInfoWarning: false

flowchartDiagrams:
  enable: false
  options: ""

sequenceDiagrams: 
  enable: false
  options: ""

---
网站换了个服务器，也懒得网站搬家了（网站账号密码忘了），以后就写博文吧，用startbbs弄个论坛也没个鸟人。

<!--more-->

以前哥在一个主机群里碰到一玩LOL韩服的家伙，碰巧我那时候迷上这游戏了，一下激起我玩韩服虐棒子的冲动，于是立马加了他好友，然后下了韩服。我找他要了个帐号，然后就开始我的生涯了。后来我建了个QQ群（139057000），到贴吧里面一发，很多人就进群了，然后无意间看到一个群里人是简体中文的界面，我就好奇了，然后经过一番询问和请教，最后终于折腾好了，韩服、美服、台服神马的，只要改一个文件就能切换着玩了，今天就是要教大家怎么弄。

1.首先登录 http://lol.garena.com/download 下载完整客户端

2.登录 http://www.garena.sg/register/ 注册一个帐号

3.安装完打开Garena，登录，然后点击左下角的设置按钮

4.按如图设置，点确定，然后退出重新打开

5.接下来没Garena的事儿了，关了吧。然后打开目录\\GameData\\Apps\\LoL\\Air，你会看见一个lol.properties的文件，删除掉。然后解压附件，将文件全部复制到此目录下，将你想玩的服的那个文件重命名为\"lol.properties\"

6.打开目录\\GameData\\Apps\\LoL，目录下有一个lol.exe的文件，点击打开，然后输入账号，进入游戏吧（简体中文哟）！