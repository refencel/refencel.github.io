---
layout: post
title: div模拟textarea实现高度自变化
categories: [HTML5]
description: 之前遇到产品提出一个需求，说是一个textarea需要动态改变高度，到一定高度后出现滚动条。当时拿到需求的时候，第一时间想到的是通过js来动态改变高度，无奈在网上都没有找到一个比较好的方法，今天在网上看到一篇使用h5特性完成，觉得挺好的就记录下来。
---

首先我们敲一个div出来
```html
<div id="textarea" contenteditable="true"></div>
```

然后就是写一些简单样式，显示出来即可
```css
#textarea{
    width: 300px;
    min-height: 150px;
    max-height: 300px;
    border: 1px solid #ccc;
    overflow: auto;
    outline: none;
    font-size: 14px;
}
```
这样我们就可以实现textarea动态改变高度了,是不是非常的简单。而且早在很早之前IE就支持了这一属性，至少IE6是没有问题的。所以兼容性都不用考虑。





