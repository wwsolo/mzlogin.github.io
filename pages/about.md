---
layout: page
title: About
description: 王大妞的博客
keywords: Wang wei, IT
comments: true
menu: 关于
permalink: /about/
---

也许曲终人散之后，

离开的离开，忘记的忘记，

然而旋律最好的时候，

感谢上天让我们在一起。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
