---
layout: default
image: https://wx3.sinaimg.cn/mw690/708e9e51ly1gcuvwmvw45j21jk0rswn6.jpg
title: 喂鲸鱼
---

{{ site. summber }} {: .aside}

<figure>
  <img src="https://wx3.sinaimg.cn/mw690/708e9e51ly1gcuvwmvw45j21jk0rswn6.jpg">
  <figcaption>卓别林第一遇见海伦凯勒</figcaption>
</figure>
{% assign note = site.data.notes[0] %}
<div class="note">
  <div class="note-heading target">最近的碎碎念 # {{ note.date | date: "%Y-%m-%d" }}</div>
  {{ note.content | markdownify }}
</div>
<ul class="terminal">
  <li><a href="/notes">More>></a></li>
</ul>