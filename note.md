---
layout: page
title: 随记
permalink: /note/
---

# 随记
共有 {{ site.note | size }} 文章

{% assign sorted_notes = site.note | sort: 'date' | reverse %}
<ul>
{% for post in sorted_notes %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span>{{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>
