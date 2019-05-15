---
title : "构建我的个人博客站点"
description: "我觉得有必要说下这个个人网站是如何建立的，以及之后可能对既有网站的设计改进。或许你也想整一个自己的个人博客，说不定有些经验和注意点可以提前知悉..."
slug: "how"
tags: ["about"]
minute: 6
date: 2019-01-12T23:15:09-07:00
related: ["/about/about1", "/about/about3"]

---


### 写在前面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我觉得有必要说下这个个人网站是如何建立的，以及之后可能对既有网站的设计改进。或许你也想整一个自己的个人博客，说不定有些经验和注意点可以提前知悉...

---

### 正文

#####  1. 选择一个网站构建工具

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;个人博客网站的搭建现在有很多方便的工具了，比如：[wordpress](https://wordpress.org)、[hexo](https://hexo.io)等等，最终我选择了[hugo](https://gohugo.io), `hugo` 是使用`golang`写的(`最近我正好在学习golang，这其实很影响我之所以选择这款工具`)一个适用于构建静态页面网站的工具，支持现在流行的**markdown**文档页面(`当然,传统的html页面也依然支持`)，官网还提供不少主题(`theme`)，可以省略个人编写大量交互`js`和`css`样式的过程(`如果想实现更加炫酷的形式，而在提供的主题中没有找到的话，还是需要自己来写了`) 。

##### 2. 选择一款主题(theme)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;这里的主题是指`hugo`构建的博客站点的主题风格，其中包括网站整体的`js`，`css`以及页面主体的视图结构和必要的静态资源文件。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`hugo`官网提供了不少不错的网站主题供我们使用或借鉴(`我主要从事后端开发，在页面设计方面的经验并不丰富`)，比如使用方便的[hyde](https://themes.gohugo.io/hyde)、简约但功能完备的[Jeffprod](https://themes.gohugo.io/hugo-blog-jeffprod/)、交互特效不错的[Meghna](https://themes.gohugo.io/meghna-hugo/)等等，我最终选择了[forty](https://themes.gohugo.io/theme/forty), 这是一款有着不错完成度的响应式分布的主题，其中也没有额外的`js`插件，十分轻量。

##### 3. 构建站点

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;现在已经可以使用主题中提供的**exampleSite**目录、借助`hugo`内置的web服务器浏览一个站点了，接着是将这移植到我们从搬瓦工([Banwagon](https://bwh88.net/cart.php))或者各大云服务器提供商那购买的VPS上了。这里我用了`nginx`作为请求分发，反向代理了`hugo server`，方便后续的扩展。(`关于nginx的使用这里不赘述了，不过有疑问依然可以留言。`)

---

### 结语

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;到此，我们已经可以通过我们VPS的IP 或者个人域名地址访问我们的个人站点了。也许，此时你还有着自己更酷的想法想改造这个站点，比如我，之前提过，我选择了[forty](https://themes.gohugo.io/theme/forty)这个主题，但这其实并不能满足我，为此，我可以加上标签(`tag`)、分页(`pagination`)，之后我还会分享我的图集(`gallery`)、Vlog等。

