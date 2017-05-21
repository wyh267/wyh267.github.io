---
layout: page
title: About
description: 什么都说的我
keywords: 没有关键词
comments: true
menu: 关于
permalink: /about/
---

老码农，求学于岳麓山脚下，混迹在帝都和杭州。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}


{% for category in site.data.skills %}
## {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
