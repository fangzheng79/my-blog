---
title: Readium:A Magic Tool that can Skip the Limitation of Medium
date: 2020-06-16
img: ./readium-logo.png 
tags: [Tools]
---

一旦涉猎的信息范围越来越广，接触到的信息平台也就越来越多。在某些特定信息来源上，国外的一些知名媒体平台开始成为优质来源之一。Medium是我最喜欢的博客平台之一，我经常在上面阅读关于技术的博文，然而这个平台只允许免费用户每个月可免费阅读 3 篇付费文章，想要继续阅读，就需要支付订阅费每个月 5 美元，实在是没（q）有（i）付（ó）费（n）欲（g）望（~_~）。

今天发现了一个神奇的小工具，名叫Readium，用来跳过部分网站的阅读限制，目前支持以下五个网站：

- 纽约时报
- Business Insider（PRIME）
- Medium
- Bloomberg
- Towards Data Science

![Readium](./readium.jpg)

使用方法很简单，访问 Readium 的网站页面，拖动页面上「Readium」的按钮放到书签栏。在访问支持的网站遇到阅读限制时，直接点击该书签按钮，网页就会自动刷新而不再有阅读限制。

对着这个原理，作者也在 Medium 上做了一些简单的说明，当你打开 Business Insider（PRIME）等网站的时候，其实可以看到文章本身已经加载完成了，但随后出现了订阅提醒的弹窗，这意味着内容本身已经加载完毕，只是被隐藏了。因此，Readium 的作用相当于「撤回」其隐藏的操作过程，从而能够直接阅读原文。

不过这个小工具应对某些网站还是有些问题，例如彭博社的文章跳过阅读限制之后，文字内容显示没问题，图片全部会变成缩略图，普通配图可能还好，但图表内容就完全看不清，直接访问图片地址也不行。

根据作者的陈述，Readium 还处于初级版本，后续会逐渐优化，此外也会根据用户反馈考虑支持更多的网站。

> Readium 地址：<https://sugoidesune.github.io/readium/>

最后附上演示视频：
<iframe width="750" height="450" src="https://www.youtube.com/embed/_5s5VUrNPMA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>