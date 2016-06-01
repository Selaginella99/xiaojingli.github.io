---
layout: single
title: "个性化配置"
categories: [blog ]
tags: [tech]
description: 



excerpt: "对照博主提供的信息进行个性化配置"
header:
  overlay_image: autumn.jpg
  teaser : "autumn.jpg"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  cta_label: "More Info "
  cta_url: "https://unsplash.com"
---

{% include toc icon="gears" title="My Table of Contents" %}

# 关于此模板的几个重要连接
---
[docs/Layouts](https://mmistakes.github.io/minimal-mistakes/docs/layouts/)

[模板仓库_pages](https://github.com/mmistakes/minimal-mistakes/tree/gh-pages/_pages)

[模板仓库_posts](https://github.com/mmistakes/minimal-mistakes/tree/gh-pages/_posts)

---



# 添加题图
```
---
layout: single
title: "个性化配置"
categories: [blog ]
tags: [tech]
description: 



excerpt: "对照博主提供的信息进行个性化配置"
header:
  overlay_image: autumn.jpg
  teaser : "autumn.jpg"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
---
```
可以自行设计rgba

```
excerpt: "This post should [...]"
header:
  overlay_image: unsplash-image-1.jpg
  overlay_filter: rgba(255, 0, 0, 0.5)
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  cta_label: "More Info"
  cta_url: "https://unsplash.com"
```

# 添加两张并列图片,画廊
```
<figure class="half">
    <a href="/images/seagulls.jpg"><img src="/images/seagulls.jpg"></a>
    <a href="/images/sky2.jpg"><img src="/images/sky2.jpg"></a>
    <figcaption>Caption describing these two images.</figcaption>
</figure>
```
<figure class="half">
    <a href="/images/seagulls.jpg"><img src="/images/seagulls.jpg"></a>
    <a href="/images/sky2.jpg"><img src="/images/sky2.jpg"></a>
    <figcaption>Caption describing these two images.</figcaption>
</figure>

值得注意的是：

```
<figcaption>Caption describing these two images.</figcaption>
```
其中添加了图形下面的文字

## 添加三张图片
```
<figure class="third">
	<img src="/images/seagulls.jpg">
	<img src="/images/sky2.jpg">
	<img src="/images/sky2.jpg">
	<figcaption>Caption describing these three images.</figcaption>
</figure>
```
<figure class="third">
	<img src="/images/seagulls.jpg">
	<img src="/images/sky2.jpg">
	<img src="/images/sky2.jpg">
	<figcaption>Caption describing these three images.</figcaption>
</figure>


# Buttons
Make any link standout more when applying the .btn class.

```
[按照目录排列](/categories/){: .btn}
[Success Button Text](/tags/){: .btn .btn--success}
[Warning Button Text](#link){: .btn .btn--warning}
[Danger Button Text](#link){: .btn .btn--danger}
[Info Button Text](#link){: .btn .btn--info}
[Inverse Button](#link){: .btn .btn--inverse}
[Light Outline Button](#link){: .btn .btn--light-outline}
```

[按照目录排列](/categories/){: .btn}
[按照标签排列](/tags/){: .btn .btn--success}
[Warning Button Text](#link){: .btn .btn--warning}
[Danger Button Text](#link){: .btn .btn--danger}
[Info Button Text](#link){: .btn .btn--info}
[Inverse Button](#link){: .btn .btn--inverse}
[Light Outline Button](#link){: .btn .btn--light-outline}

```
[X-Large Button](#link){: .btn .btn--x-large}
[Large Button](#link){: .btn .btn--large}
[Default Button](#link){: .btn}
[Small Button](#link){: .btn .btn--small}
```

[X-Large Button](#link){: .btn .btn--x-large}
[Large Button](#link){: .btn .btn--large}
[Default Button](#link){: .btn}
[Small Button](#link){: .btn .btn--small}

# 调整图片的位置
<img src="/images/hacker.png" width="150" height="150" alt="hacker"/>{: .align-right} 
<img src="/images/hacker.png" width="150" height="150" alt="hacker"/>{: .align-left}
<img src="/images/hacker.png" width="150" height="150" alt="hacker"/>{: .align-center}  

```
<img src="/images/hacker.png" width="150" height="150" alt="hacker"/>{: .align-right} 
<img src="/images/hacker.png" width="150" height="150" alt="hacker"/>{: .align-left}
<img src="/images/hacker.png" width="150" height="150" alt="hacker"/>{: .align-center} 
```
单独使用 `{: .align-right}` 的效果如下图：
<img width="812" alt="2016-05-31 22 06 34" src="https://cloud.githubusercontent.com/assets/11477264/15688785/0003f594-277c-11e6-8636-3aeaaf1cc2fc.png">

# 关于目录
1. 会影响代码的现实
2. 目录旁可以放置文字内容，其他的就算了吧……

End.

> 20160531 搭建博客，粗浅地学习博主讲到的内容