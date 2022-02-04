---
title: 记录被“git pull --rebase origin master”坑的一天
date: 2022-02-04 22:58:15
cover: /covers/cover-5.jpg
categories:
- 日常
tags:
- 踩坑
excerpt: 起因 记得那时一个天气晴朗的上午...
---

## 起因
记得那时一个天气晴朗的上午，我打开了电脑，准备将自己的Vue项目托管到github上，结果push的时候报错了，于是我就去必应寻找解决办法，说是用什么`git pull --rebase origin master`，我去试了一下，才发现我被骗了，代码回到了很久之前的样子，我直接崩溃了。。。

## 解决方法
先使用`git reflog --date=iso`查看操作日志
然后再`git reset --hard {id}`进行操作，id是日志里显示的（记得找pull前的那一个）
最后你就愉快的发现你的代码回来咯！
