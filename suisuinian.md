---
layout: default
title: 长话短说
image: https://wx3.sinaimg.cn/mw690/708e9e51ly1gcuvwmvw45j21jk0rswn6.jpg
---
{% for note in site.notes reversed %}
<div class="aside-tweet" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">
  <div class="date">
    <date>
      <small>
        <a href="#date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">{{ note.date | date: "%Y-%m-%d %H:%M"}}</a>
      </small>
    </date>
  </div>
  {{ note.content | markdownify }}
</div>
{% endfor %}
