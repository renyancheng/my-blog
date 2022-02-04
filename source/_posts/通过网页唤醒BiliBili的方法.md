---
title: 通过网页唤醒BiliBili的方法
date: 2022-02-04 18:52:49
categories:
- web前端
tags: 
- BiliBili
- Url
# cover: https://api.yimian.xyz/img?type=moe
cover: /covers/cover-2.jpg
excerpt: 前言 大家应该都知道在浏览器中输入...
---
## 前言
大家应该都知道在浏览器中输入
```
mqq://
```
来打开QQ，那么我就想，哔哩哔哩有没有这个东西呢，于是经过一番研究，发现了这个。
## 协议
通过网页唤醒哔哩哔哩的协议统一为
```
bilibili://
```
## 方法
### 打开APP主页
```
bilibili://home
```
### 打开用户页面
```
bilibili://space/{uid}
```
### 打开视频播放界面
```
bilibili://video/{av}or{bv}
```
### 打开搜索页面
```
bilibili://search
```
如果想加上关键词？
```
bilibili://search/?keyword={keyword}
```
### 打开直播间
```
bilibili://live/{id}
```

暂且发现这些，如果你有了新的发现一定要告诉我～