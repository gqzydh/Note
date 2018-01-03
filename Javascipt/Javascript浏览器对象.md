
---
title: Javascript浏览器对象
date: 2017-10-17 14:51:01
tags:
- Javascript
- 笔记
categories: 
- Javascript
---


## 计时方法：
```
1）：setInterval() 间隔指定的毫秒数不停地执行指定的代码
clearInterval()  方法用于停止setIntearval()方法执行的函数代码

2）：setTimeout() 暂停指定的毫秒数后执行指定的代码
clearTimeout()  方法用于停止执行setTimeout() 方法的函数代码

History 对象包含浏览器的历史（url）的集合
history.back()  与在浏览器点击后退按钮相同
history.forward() 与在浏览器中点击按钮向前相同
history.go()  进入历史中的某个页面

Location 对象用于获取得当前页面的地址（URL），并把浏览器重定向到新的页面
属性：location.hostname  返回web主机的域名
        location.pathname  返回当前页面的路径和文件名
        location.pry 返回web主机的端口
        location.protocol  返回所使用的web协议（http://或https://）
        location.href  属性返回当前页面的URL
        location.assign()  方法加载新的文档

screen  对象包含有关用户屏幕的信息
    screen,availWidth   可用的屏幕宽度
    screen.availHeight   可用的屏幕高度
    screen.height    屏幕高度
    screen.width      屏幕宽度
```