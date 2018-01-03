
---
title: Ajax笔记 
date: 2017-10-17 14:51:01
tags:
- Ajax 
- 笔记
categories: 
- Ajax 
---


```
responseText： //获得字符串形式的响应数据
responseXML： //获得 XML 形式的响应数据
```
##Ajax ajax readyState的五种状态详解##
0 － （未初始化）还没有调用send()方法 
1 － （载入）已调用send()方法，正在发送请求 
2 － （载入完成）send()方法执行完成，已经接收到全部响应内容 
3 － （交互）正在解析响应内容 
4 － （完成）响应内容解析完成，可以在客户端调用了

## Jquery ajax 例子详解 ##
```
function test(){
   $.ajax({
            //提交数据的类型 POST GET
            type:"POST",
            //提交的网址
            url:"testLogin.aspx",
            //提交的数据
            data:{Name:"sanmao",Password:"sanmaoword"},
            //返回数据的格式
            datatype: "html",//"xml", "html", "script", "json", "jsonp", "text".
            //在请求之前调用的函数
            beforeSend:function(){$("#msg").html("logining");},
            //成功返回之后调用的函数             
            success:function(data){
           $("#msg").html(decodeURI(data));            
            }   ,
            //调用执行后调用的函数
            complete: function(XMLHttpRequest, textStatus){
               alert(XMLHttpRequest.responseText);
               alert(textStatus);
                //HideLoading();
            },
            //调用出错执行的函数
            error: function(){
                //请求出错处理
            }         
         });

  }
```