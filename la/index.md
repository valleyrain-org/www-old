---
layout: page
title: "LA分部活动"
description: "谷雨书苑LA分部活动页面"
pos: "3"
---

<div class="tiles">
{% for post in site.categories.la %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->
