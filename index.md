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
{% assign note = site.notes[0] %}
<div class="tweeter-tweet">
  <div class="date">最近的碎碎念 # {{ note.date | date: "%Y-%m-%d" }}</div>
  {{ note.content | markdownify }}
</div>
<ul class="terminal">
  <li><a href="/suisuinian">More>></a></li>
</ul>