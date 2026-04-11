---
layout: default
title: Tech Trend Daily
---

# Tech Trend Daily 🚀

매일 아침 최신 기술 트렌드와 유망 주식을 분석해드립니다.

> 본 블로그의 주식 분석은 투자 참고용이며 투자 권유가 아닙니다.

## 최신 글 목록

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}