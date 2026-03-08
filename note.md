---
layout: default
title: 随记
permalink: /note/
---

# 随记

<ul>
{% for post in site.note %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span>{{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>
