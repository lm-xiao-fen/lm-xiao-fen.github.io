---
layout: default
title: 随记
---

# 随记

这里记录一些日常想法、折腾记录与零碎笔记。

<ul class="list-style-none pl-0">
  {% for post in site.categories.note %}
    <li class="mb-3">
      <h3 class="mb-1">
        <a class="link-gray-dark" href="{{ post.url }}">
          {{ post.title }}
        </a>
      </h3>
      <div class="text-small color-fg-muted">
        {{ post.date | date: "%Y-%m-%d" }}
      </div>
      {% if post.excerpt %}
      <div class="mt-1 text-small">
        {{ post.excerpt | strip_html | truncate: 120 }}
      </div>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% if site.categories.note == nil %}
<p class="color-fg-muted">暂无随记</p>
{% endif %}