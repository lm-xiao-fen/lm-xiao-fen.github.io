---
layout: default
title: 技术博客
---
### [xf_blog](/)    

# 技术博客

<ul class="list-style-none pl-0">
  {% for post in site.posts %}
    <li class="mb-3">
      <h3 class="mb-1">
        <a href="{{ post.url }}" class="link-primary">
          {{ post.title }}
        </a>
      </h3>
      <div class="text-small color-fg-muted">
        {{ post.date | date: "%Y-%m-%d" }}
      </div>
    </li>
  {% endfor %}  
</ul>

### 联系我
[bilibili](https://space.bilibili.com/3494372658121066/)  
[email:G114514g@yeah.net](mailto:G114514g@yeah.net)  
[YouTube](https://youtobe.com/@lm-xiao-fen)
