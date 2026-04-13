---
layout: default
title: 카테고리
permalink: /categories/
---

## 📂 카테고리

{% assign categories = site.categories | sort %}
{% for category in categories %}
<h3>{{ category[0] }} ({{ category[1].size }})</h3>
<ul>
  {% for post in category[1] %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
  {% endfor %}
</ul>
{% endfor %}