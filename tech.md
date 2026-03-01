---
layout: default
title: 技术博客
permalink: /tech/
---

# 技术博客

<ul>
{% for post in site.posts %}
  {% if post.path contains '_posts/tech/' %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endif %}
{% endfor %}
</ul>
