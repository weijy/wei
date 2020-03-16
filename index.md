---
layout: default
image: /images/front.jpg
---

<ul class="list pa0">
        {% for post in site.posts %}
        <li class="mb4-l mb3">
            <span class="ttu f7 b mr2 tracked grey db-l dn">{{ post.date | date: '%Y/%m/%d' }}</span>
            
            <a href="{{ post.url }}" class="f4">{{ post.title }}</a>
        </li>
        {% endfor %}
</ul>