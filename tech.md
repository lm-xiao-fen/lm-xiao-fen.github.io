---
layout: page
title: 技术博客
permalink: /tech/
---

# 技术博客

{% assign tech_posts = site.posts 
  | where_exp:"post","post.path contains '_posts/tech/'" 
  | sort: "date" 
  | reverse %}

<p>共有 {{ tech_posts | size }} 篇</p>

<ul>
{% for post in tech_posts limit %}
  <li style="margin-bottom:6px;">
    <span style="color:#8b949e; font-size:13px;">
      {{ post.date | date: "%Y-%m-%d" }}
    </span>
    <a href="{{ post.url }}" style="margin-left:6px;">
      {{ post.title }}
    </a>
  </li>
{% endfor %}
</ul>