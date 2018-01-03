---
title: JQuery常用方法
date: 2017-10-17 14:51:01
tags:
- JQuery
- 笔记
categories: 
- JQuery
---


```
addClass()  //方法给元素加class
removeClass()  //方法删除元素的class。
```

## css ##
```
$("#tag").css("color", "blue");
$("#tag").css({"width":"200px","color":"blue"});

$(".target:nth-child(3)").addClass("animated bounce");
target:nth-child(n) //CSS选择器允许你通过目标类或元素类型选择目标元素的所有子元素。

$(".target:odd").addClass("animated shake");  //获取所有奇数元素
$(".target:even").addClass("animated shake"); //获取所有偶数元素
```

```
$("button").prop("disabled", true);  //禁用按钮,按钮会变灰并且不能点击

$("h3").html("<em>jQuery Playground</em>");  //在元素中添加HTML标签和文字，而元素中之前的内容都会被方法中的内容所替换掉
 .text()  //改变文本但不能添加标签。
 $("#target4").remove()  //的方法，可以彻底删除一个HTML元素。
 appendTo()  //方法，可以让你把选中的HTML元素附加到其他元素中。
 $("#target2").clone().appendTo("#right-well");  //可以复制元素。再添加到

 $("#left-well").parent().css("background-color", "blue")  //可以允许你访问选定元素的父元素。并从中继承属性。
 children(子元素)， //子元素从父元素那里继承属性。
```