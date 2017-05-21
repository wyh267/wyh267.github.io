---
layout: page
title: Wiki
description: 这里就是一些笔记和转帖,还没到写Blog的程度
keywords: 维基, Wiki
comments: false
menu: 维基知识库
permalink: /wiki/
---

> 记多少命令和快捷键会让脑袋爆炸呢？

<ul class="listing">
{% for wiki in site.wiki %}
{% if wiki.title != "Wiki Template" %}
<li class="listing-item"><a href="{{ wiki.url }}">{{ wiki.title }}</a></li>
{% endif %}
{% endfor %}
</ul>
