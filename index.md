---
layout: default
title: xf_blog
---
# Hi, I'm xiaofen（lm-xiao-fen）

- 欢迎来到我的个人主页
- 这里记录我在 **Web 开发 / Cloudflare / GitHub /视频创做** 方面的内容
- [副站](https://lm-xiao-fen.github.io/my-web/)

## 联系我

[bilibili](https://space.bilibili.com/3494372658121066)
[Email](mailto:G114514g@yeah.net)
[YouTube](https://youtube.com/@lm-xiao-fen)

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

[查看全部技术博客](/tech)

---

## 最新随笔

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

[查看全部随笔](/note)
