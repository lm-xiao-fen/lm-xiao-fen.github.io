---
layout: default
title: xf_blog      
---

# 👋 Hi, I'm lm-xiao-fen  

欢迎来到我的个人主页
这里记录我在 **Web 开发 / Cloudflare / 学习笔记** 方面的内容
[副站](https://lm-xiao-fen.github.io/my-web)    

---

## 📝 Blog

<ul class="list-style-none pl-0">
  {% for post in site.posts %}
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

{% if site.posts.size == 0 %}
<p class="color-fg-muted">
  还没有文章，敬请期待 👀
</p>
{% endif %}  

### 联系我
[bilibili](https://space.bilibili.com/3494372658121066)        
