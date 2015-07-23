---
layout: page
title: "活动回顾"
description: "This is what I do."
header-img: "img/about-bg.jpg"
pos: "2"
---

<div class="tiles">
{% for post in site.categories.event %} {% if post.date < site.time %}
  {% include archive-tiles.html %}
{% endif %} {% endfor %}
</div><!-- /.tiles -->
