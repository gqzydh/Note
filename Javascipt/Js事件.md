
---
title: Js事件
date: 2017-10-17 14:51:01
tags:
- Javascript
- 笔记
categories: 
- Javascript
---


## input 触发事件
```
onkeyup 事件会在键盘按键被松开时发生。
输入您的姓名： <input type="text" id="fname" onkeyup="upperCase(this.id)" />
onClick   单击事件
onMouseOver    鼠标经过事件
onMouseOut    鼠标移出事件
onChange  文本内容改变事件
onSelect    文本框选中事件
onFocus    光标聚集事件
onBlur      移开光标事件
onLoad     网页加载事件
onUnload    关闭网页事件
```
## 防止网页被嵌入框架的代码
```
<script type="text/javascript">
if (window!=top) // 判断当前的window对象是否是top对象
top.location.href =window.location.href; // 如果不是，将top对象的网址自动导向被嵌入网页的网址
</script>
```
>  改进使得我的网页只能被嵌入我自己的框架，而不是别人的框架？
```
<script type="text/javascript">
try{
　　top.location.hostname;
　　if (top.location.hostname != window.location.hostname) {
　　　　top.location.href =window.location.href;
　　}
}
catch(e){
　　top.location.href = window.location.href;
}
</script>

```
