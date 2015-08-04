---
layout: page
title: "绘画作品"
description: "网友原创绘画作品"
pos: "4"
---

<div class="tiles">
{% for post in site.categories.painting %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->
