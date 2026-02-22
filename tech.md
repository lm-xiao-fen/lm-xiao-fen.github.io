---
layout: default
title: 技术博客
---

# 技术博客

<ul class="list-style-none pl-0">
  {% for post in site.categories.tech %}
    <li class="mb-3">
      <h3 class="mb-1">
        <a class="link-gray-dark" href="{{ post.url }}">
          {{ post.title }}
        </a>
      </h3>
      <div class="text-small color-fg-muted">
        {{ post.date | date: "%Y-%m-%d" }}
      </div>
    </li>
  {% endfor %}
</ul>