---
layout: page
image: http://wx1.sinaimg.cn/large/708e9e51ly1gcy0cyckswj21hc0u0n66.jpg
title: 长话短说
title-hide: true
---
{% for note in site.notes reversed %}
<div class="note" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">
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
