---
layout: default
image: https://wx3.sinaimg.cn/mw690/708e9e51ly1gcuvwmvw45j21jk0rswn6.jpg
---
{% for note in site.notes reversed %}
<div class="aside" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">
  <div class="date">
    <date>
      <small>
        <a class="no-border" href="{{ note.url }}">{{ note.date | date: "%Y-%m-%d %H:%M"}}</a>
      </small>
    </date>
  </div>
  {{ note.content | markdownify }}
</div>
{% endfor %}
