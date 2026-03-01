---
layout: default
title: 技术博客
permalink: /tech/
---

# 技术博客

<p>共有 {{ site.posts | size }} 篇文章</p>

<ul>
{% for post in site.posts %}
  <li>
    {{ post.title }} - {{ post.url }}
  </li>
{% endfor %}
</ul>
