---
layout: default
title: LP Letter
permalink: /blog
active: blog
---
<div class="section list">
  <h1>LP Letter</h1>
  <p class="meta">분기별 실험/투자 업데이트. 실패도 포함합니다.</p>
  <ul class="list">
  {% for post in site.posts %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <span class="meta">· {{ post.date | date: "%Y.%m.%d" }}</span></li>
  {% endfor %}
  </ul>
</div>