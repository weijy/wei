---
layout: default
title: 长话短说
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
