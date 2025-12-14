---
layout: default  
title: xf_blog 
---

# Hi, I'm lm-xiao-fen

欢迎来到我的个人主页。  
这里记录我在 **Web 开发 / Cloudflare / GitHub / UP 主 / YouTuber** 方面的内容。

[副站](https://lm-xiao-fen.github.io/my-web/index.html)  

---

## Blog  

<ul class="list-style-none pl-0">
  {% for post in site.posts %}
    <li class="mb-4">
      <div class="mb-1">
        <a class="link-gray-dark h3" href="{{ post.url }}">
          {{ post.title }}
        </a>
      </div>

      <div class="text-small color-fg-muted mb-1">
        {{ post.date | date: "%Y-%m-%d" }}
      </div>

      {% if post.excerpt %}
      <div class="text-small color-fg-muted">
        {{ post.excerpt | strip_html | truncate: 80 }}
      </div>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% if site.posts.size == 0 %}
<p class="color-fg-muted">
  还没有文章，敬请期待
</p>
{% endif %}

---

## 联系我

- [bilibili](https://space.bilibili.com/3494372658121066)
- [email: G114514g@yeah.net](mailto:G114514g@yeah.net)
- [YouTube](https://youtube.com/@lm-xiao-fen)
