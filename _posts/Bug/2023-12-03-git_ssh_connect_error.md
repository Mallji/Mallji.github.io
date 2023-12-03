---
layout: post
title: 'git连接被关闭'
tags: Bug
image: /public/images/sierra.jpg
---
今天遇到了一个在使用git的时候遇到的bug
```shell
Connection closed by 198.18.0.112 port 22
```
发现这个ip是一个私有ip
经过摸索发现是自己使用Clash for windows的时候开启了Tun模式(好像开启这个模式之clash创建了一张虚拟网卡)
所以只要关闭TUN模式就可以了,在需要的时候打开TUN模式
具体什么原因不知道,等到以后有时间再来研究