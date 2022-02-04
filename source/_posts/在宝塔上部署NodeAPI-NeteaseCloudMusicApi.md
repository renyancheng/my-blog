---
title: 在宝塔上部署NodeAPI-NeteaseCloudMusicApi
date: 2022-02-04 23:09:02
cover: /covers/cover-4.jpg
categories:
- 教程分享
tags:
- 宝塔
- 网易云音乐
- API接口
excerpt: 首先，下载这个源码 https://github.com/Binar...
---
# 安装

首先，下载这个源码
https://github.com/Binaryify/NeteaseCloudMusicApi

<!-- ![](https://mf.xgzwlkj.cn/wp-content/uploads/2021/04/1617687002463-138x300.jpg) -->

当然在服务器终端上直接git clone也是可以的！

我这边直接下载上传到了www目录下，然后解压Zip。

<!-- ![](https://mf.xgzwlkj.cn/wp-content/uploads/2021/04/1617687003315-159x300.png) -->

# 宝塔上配置
打开宝塔软件商店安装PM2管理器，然后打开设置选择你解压项目的文件夹，启动文件名称填写app.js，项目名称随便填写一个就行，然后点添加，添加成功后先不要管，点击侧边栏的安全，放行3000端口（该项目默认运行在3000端口）。

<!-- ![](https://mf.xgzwlkj.cn/wp-content/uploads/2021/04/1617687004362-159x300.png) -->
<!-- ![](https://mf.xgzwlkj.cn/wp-content/uploads/2021/04/1617687005318-162x300.png) -->

# 终端操作
然后我们使用打开服务器终端，cd到解压的目录下，输入npm install，等待一会完成即可，然后我们回到宝塔的PM2管理器点击启动，这个接口服务就跑起来了，但是我们要怎么访问呢？

<!-- ![](https://mf.xgzwlkj.cn/wp-content/uploads/2021/04/1617687006176-248x300.png) -->

# 启动完成

启动成功后，点击映射，绑定你的域名/IP就OK！

然后访问 http://域名/IP:3000/ 可以看到已经可以使用了

<!-- ![](https://mf.xgzwlkj.cn/wp-content/uploads/2021/04/Screenshot_20210406_132318-300x140.jpg) -->

~~搭建好的站点：[http://ncmapi.li1.fun:3000/](http://ncmapi.li1.fun:3000/)(域名已到期👀)~~

接口文档：[https://binaryify.github.io/NeteaseCloudMusicApi/](https://binaryify.github.io/NeteaseCloudMusicApi/)

这个项目上百个接口，你可以用来开发另一个Web网易云音乐或者是安卓APP也可以是微信小程序这都取决于你。