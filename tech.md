---
layout: default
title: 技术博客
permalink: /tech/
---

# 技术博客

{% assign tech_posts = site.posts | where_exp:"post","post.path contains '_posts/tech/'" %}

<p>共有 {{ tech_posts | size }} 篇博客</p>

<ul>
{% for post in tech_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span>{{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>
