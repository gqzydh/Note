
---
title: CSS样式表重置 
date: 2017-10-17 14:51:01
tags:
- reset.css 
categories: 
- css 
---

1. reset.css
2. CSS样式表重置

## reset.css ##
```
/* reset.css（格式化样式） */
@charset "utf-8";
html{background:#fff;overflow:auto;}
body{min-width:1200px;font:12px/18px "Microsoft Yahei";font-weight:lighter;color:#333; -webkit-font-smoothing: antialiased; }
a{color:#333; text-decoration:none; cursor:pointer; outline: 0 none;}
a:hover{ text-decoration:none;color:#ff4f20;}
a:focus{-moz-outline-style:none; border:0px;blr:expression(this.onFocus=this.blur());}
body,div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,h5,h6,pre,code,form,fieldset,legend,input,p,blockquote,th,td{margin:0; padding:0;}
header,footer,article,aside,section,nav,menu,hgroup,details,dialog,figure,figcaption{display:block}
ol,li,ul,dl,dt,dd{list-style:none;}
fieldset,img {border:0}
button,submit,input,select { vertical-align:middle;}
button,submit { cursor:pointer;}
h1,h2,h3,h4,h5,h6{font-size:inherit; font-weight:lighter;}
table{border-collapse:collapse; border-spacing:0;}
sup{vertical-align:text-top;}
sub{vertical-align:text-bottom;}
select,button{font-family:inherit; font-size:inherit; font-weight:inherit; outline-style:none; outline-width:0pt; padding: 0; margin: 0;}
b,em,i{display:inline-block; font-weight:normal; font-style:normal;}
.clearfix:after { content: "."; display: block; height: 0; clear: both; visibility: hidden;} .clearfix{ zoom:1;}
.container { width:1200px; position:relative; margin:0 auto;}
.fl{float:left;}
.fr{float:right;}
```

## CSS样式表重置 ##
```
.clearfix:before, .clearfix:after { content: ""; display: table }
.clearfix:after { clear: both }
html, body { height: 100% }
html { font-family: "Helvetica Neue", Helvetica, STHeiTi, Arial, sans-serif; -ms-text-size-adjust: 100%; -webkit-text-size-adjust: 100%; font-size: 62.5% }
body { margin: 0; font-size: 1.4rem; line-height: 1.5; color: #333; background-color: #fff }
article, aside, details, figcaption, figure, footer, header, hgroup, main, nav, section, summary { display: block }
audio, canvas, progress, video { display: inline-block; vertical-align: baseline }
audio:not([controls]) { display: none; height: 0 }
[hidden], template {
display: none
}
a { background: transparent; text-decoration: none; -webkit-tap-highlight-color: transparent; color: #08c }
a:active { outline: 0 }
a:active { color: #069 }
abbr[title] { border-bottom: 1px dotted }
b, strong { font-weight: bold }
dfn { font-style: italic }
mark { background: #ff0; color: #000 }
small { font-size: 80% }
sub, sup { font-size: 75%; line-height: 0; position: relative; vertical-align: baseline }
sup { top: -0.5em }
sub { bottom: -0.25em }
img { border: 0; vertical-align: middle }
svg:not(:root) { overflow: hidden }
hr { -moz-box-sizing: content-box; box-sizing: content-box; height: 0 }
pre { overflow: auto; white-space: pre; white-space: pre-wrap; word-wrap: break-word }
code, kbd, pre, samp { font-family: monospace, monospace; font-size: 1em }
button, input, optgroup, select, textarea { color: inherit; font: inherit; margin: 0 }
button { overflow: visible }
button, select { text-transform: none }
button, html input[type="button"], input[type="reset"], input[type="submit"] { -webkit-appearance: button; cursor: pointer }
button[disabled], html input[disabled] { cursor: default }
button::-moz-focus-inner, input::-moz-focus-inner {
border: 0;
padding: 0
}
input { line-height: normal }
input[type="checkbox"], input[type="radio"] { box-sizing: border-box; padding: 0 }
input[type="number"]::-webkit-inner-spin-button, input[type="number"]::-webkit-outer-spin-button {
height: auto
}
input[type="search"] { -webkit-appearance: textfield; -moz-box-sizing: border-box; -webkit-box-sizing: border-box; box-sizing: border-box }
input[type="search"]::-webkit-search-cancel-button, input[type="search"]::-webkit-search-decoration {
-webkit-appearance: none
}
fieldset { border: 1px solid #c0c0c0; margin: 0 2px; padding: 0.35em 0.625em 0.75em }
legend { border: 0; padding: 0 }
textarea { overflow: auto; resize: vertical }
optgroup { font-weight: bold }
table { border-collapse: collapse; border-spacing: 0 }
td, th { padding: 0 }
html, button, input, select, textarea { font-family: "Helvetica Neue", Helvetica, STHeiTi, Arial, sans-serif }
h1, h2, h3, h4, h5, h6, p, figure, form, blockquote { margin: 0 }
ul, ol, li, dl, dd { margin: 0; padding: 0 }
ul, ol { list-style: none outside none }
h1, h2, h3 { line-height: 2; font-weight: normal }
h1 { font-size: 1.8rem }
h2 { font-size: 1.6rem }
h3 { font-size: 1.4rem }
input::-moz-placeholder, textarea::-moz-placeholder {
color: #ccc
}
input:-ms-input-placeholder, textarea:-ms-input-placeholder {
color: #ccc
}
input::-webkit-input-placeholder, textarea::-webkit-input-placeholder {
color: #ccc
}
* { -webkit-box-sizing: border-box; -moz-box-sizing: border-box; box-sizing: border-box }
```
