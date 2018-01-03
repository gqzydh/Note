
---
title: Template.js 
date: 2017-10-17 14:51:01
tags:
- Template
- 笔记
categories: 
- Template 
---


### 常用语法.
```
<# print(self.makeexpect.expect); #>万  //输出金额

// if 判断
<#if(self.makeexpect.description == 1){#>
<div class="tenprizeimg"><img src="/static/img/mystory/img1.png" alt=""></div>
<#}#>
<#if(self.makeexpect.description == 2){#>
<div class="tenprizeimg"><img src="/static/img/mystory/img2.png" alt=""></div>
<#}#>
<#if(self.makeexpect.description == 3){#>
<div class="tenprizeimg"><img src="/static/img/mystory/img3.png" alt=""></div>
<#}#>
```