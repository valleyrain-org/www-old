---
layout: home
description: "读书活动列表"
---


<div class="index-content event">
    <div class="tiles">
        <ul class="artical-list">
        {% for post in site.categories.event %}
            <li>
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
            </li>
        {% endfor %}
        </ul>
    </div>
</div>
