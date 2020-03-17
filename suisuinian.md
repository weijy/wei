---
layout: default
title: 长话短说
---
{% for note in site.notes reversed %}
<div class="tweeter-tweet" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">
  <div class="date">
    <date>
    <a href="#date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">{{ note.date | date: "%Y-%m-%d %H:%M"}}</a>
    </date>
  </div>
  {{ note.content | markdownify }}
</div>
{% endfor %}
