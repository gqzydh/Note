
---
title: Javascript高级技巧
date: 2017-10-17 14:51:01
tags:
- Javascript
- 笔记
categories: 
- Javascript
---


## 输出数组里指定的
```
var arr1 = [[1, 4, 3], [4, 6, 6], [7, 20, 9]]     
$.each(arr1, function(i, item){     
   alert(item[0]);     
});  
```
## push()函数追加数组数据
```
var arr = [1,2,3];
arr.push(4);
// 现在arr的值为 [1,2,3,4]
```
```
pop()函数弹出数组最后数据
shift()函数移出数组第一个数据
unshift()函数移入数据到数组第一位
var myArray = [["John", 23], ["cat", 2]];
var re01 = myArray.pop(); //myArray=[["John", 23]\
var re02 = myArray.shift(); //re01 =  ["cat", 2 \
```
```
object.hasOwnProperty(proName)  //确定某个对象是否具有带指定名称的属性。返回true或false
```
random()生成随机小数
 ```
 Math.random()  //用来生成一个在0(包括0)到1(不包括1)之间的随机小数
 Math.floor() //向下取整 获得它最近的整数。
 Math.floor(Math.random() * 20); //获得了一个在0到19之间的整数。
 ```
 ```
 Math.floor(Math.random() * (max - min + 1)) + min //生成的随机数是在两个指定的数之间。
 ```