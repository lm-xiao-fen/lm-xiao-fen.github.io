---
layout: home
title: xf_blog
---
# [xf_blog](/)  [友链](/feed-link)

# Hi, I'm lm-xiao-fen

- 欢迎来到我的个人主页
- 这里记录我在 **Web 开发 / Cloudflare / GitHub** 方面的内容
- [副站](https://mikufans1.dpdns.org)
- [友链](/feed-link)

---

## 最新技术博客

<ul class="list-style-none pl-0">
  {% for post in site.posts limit:2 %}
    <li class="mb-3">
      <h3 class="mb-1">
        <a class="link-primary" href="{{ post.url }}">
          {{ post.title }}
        </a>
      </h3>
      <div class="text-small color-fg-muted">
        {{ post.date | date: "%Y-%m-%d" }}
      </div>
      {% if post.excerpt %}
      <div class="mt-1 text-small">
        {{ post.excerpt | strip_html | truncate: 100 }}
      </div>
      {% endif %}
    </li>
  {% endfor %}
</ul>

[技术](/tech)

---

## 最新随记

<ul class="list-style-none pl-0">
  {% assign notes = site.note | sort: "date" | reverse %}
  {% for post in notes limit:2 %}
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
        {{ post.excerpt | strip_html | truncate: 100 }}
      </div>
      {% endif %}
    </li>
  {% endfor %}
</ul>

[随笔](/note)

---

## 联系我

- [bilibili](https://space.bilibili.com/3494372658121066)
- [Email](mailto:G114514g@yeah.net)
- [YouTube](https://youtube.com/@lm-xiao-fen)
