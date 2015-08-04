---
layout: page
title: "往期笔记"
description: "往期笔记整理"
pos: "3"
---

<div class="tiles">
{% for post in site.categories.note %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->
