
---
title: Aos使用方法 
date: 2017-10-17 14:51:01
tags:
- css3动画插件
- css3
categories: 
- 插件 
---


aos.js是一款效果超赞的页面滚动元素动画jQuery动画库插件。该动画库可以在页面滚动时提供28种不同的元素动画效果，以及多种easing效果。在页面往回滚动时，元素会恢复到原来的状态。

##安装##
可以通过bower来安装aos动画库插件。

```
bower install aos --save
```

##使用方法##
在页面中引入aos.css文件,jquery和aos.js文件

```
<link rel="stylesheet" href="dist/aos.css" />
<script src="js/jquery.min.js"></script>
<script src="dist/aos.js"></script>
```

##HTML结构##
要使用aos动画库，你需要做的就是在需要动画的元素上添加aos属性，例如：

```
<div aos="animation_name">
```

aos脚本将会在页面滚动时，在该元素上触发相应的动画。
在元素上还可以添加以下一些属性：

属性  属性  属性  默认值
`aos-offset`  是立刻触发动画还是在指定时间之后触发动画    200 120
`aos-duration`    动画持续时间  600 400
`aos-easing`  动画的easing动画效果   ease-in-sine    ease
`aos-delay`  动画的延迟时间 300 0
`aos-anchor`  锚元素。使用它的偏移来取代实际元素的偏移来触发动画   #selector   null
`aos-anchor-placement`   锚位置，触发动画时元素位于屏幕的位置  top-center  top-bottom
`aos-once`    动画是否只会触发一次，或者每次上下滚动都会触发 true    false

> 注意，aos-duration的动画持续时间的范围从50-3000毫秒，如果你想设置更大的值，可以在页面中添加下面的CSS代码：

```
body[aos-duration='4000'] [aos], [aos][aos][aos-duration='4000']{
  transition-duration: 4000ms;
}
// 上面的代码将动画的持续时间修改为4000毫秒。
```

## 示例代码：##

```
<div aos="fade-zoom-in" aos-offset="200" aos-easing="ease-in-sine" aos-duration="600">
<div aos="flip-left" aos-delay="100" aos-anchor=".example-selector">
<div aos="fade-up" aos-anchor-placement="top-center">
```
如果你担心HTML5校验的问题，可以为上面的属性添加data-前缀。

```
<div data-aos="animation_name" data-aos-offset="200" data-aos-easing="ease-in-sine">

```

##全局配置##
如果你不想单独每个元素做一个动画配置，你可以通过init()方法来统一配置所有元素的动画效果。

```
AOS.init({
  offset: 200,
  duration: 600,
  easing: 'ease-in-sine',
  delay: 100,
});
```

##额外配置##
AOS提供了2个额外的配置方法，这些方法只能够在初始化时使用。
配置  描述  示例值 默认值
`disable` AOS被禁用的条件   mobile  false
`startEvent`  AOS被初始化的事件名称    exampleEvent    DOMContentLoaded

##禁用AOS：##
如果你项在小屏幕设备中禁用AOS，可以：

```
AOS.init({
  disable: 'mobile'
});
```
你可以传入3种设备的类型：mobile、phone或tablet。
你也可以设置自己的禁用条件，例如在屏幕小于1024像素时禁用AOS：

```
disable: window.innerWidth < 1024
```

或者传入一个函数，返回true或false。

```
disable: function () {
    var maxWidth = 1024;
    return window.innerWidth < maxWidth;
}
```

##开始动画的事件：##
如果你不想滚动动画从页面加载（DOMContentLoaded）后就开始执行，可以使用startEvent来设置自己的事件，AOS会在document上监听这个事件：

```
AOS.init({
  startEvent: 'someCoolEvent'
});
```

## API##
AOS对象有2个可用的方法：
- init
- refresh

```
AOS.refresh();
```
上面的代码会重新计算元素的位置和偏移。

##动画和锚位置##
- 动画
    - 淡入淡出动画

```
fade-up

fade-down

fade-left

fade-right

fade-up-right

fade-up-left

fade-down-right

fade-down-left
```

    - 翻转动画

```
flip-up

flip-down

flip-left

flip-right
```

    - 滑动动画

```
slide-up

slide-down

slide-left

slide-right
```

    - 缩放动画：

```
zoom-in

zoom-in-up

zoom-in-down

zoom-in-left

zoom-in-right

zoom-out

zoom-out-up

zoom-out-down

zoom-out-left

zoom-out-right
```

    - 锚位置

```
top-bottom

top-center

top-top

center-bottom

center-center

center-top

bottom-bottom

bottom-center

bottom-top

easing动画
```

    - 你可以使用以下的一些easing动画效果：

```
linear

ease

ease-in

ease-out

ease-in-out

ease-in-back

ease-out-back

ease-in-out-back

ease-in-sine

ease-out-sine

ease-in-out-sine

ease-in-quad

ease-out-quad

ease-in-out-quad

ease-in-cubic

ease-out-cubic

ease-in-out-cubic

ease-in-quart

ease-out-quart

ease-in-out-quart
```