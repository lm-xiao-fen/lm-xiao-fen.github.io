---
layout: home
title: xf_blog
permalink: /
---
### [xf_blog](/)&emsp;[副站](https://mikufans1.dpdns.org)&emsp;[友链](/feed-link/)&emsp;[归档](/archive/)&emsp;[标签](/tag/)

# Hi, I am xiaofen

- 欢迎来到我的个人主页
- 这里记录我在 **开发 / 生活** 方面的内容

---
## tech

{% assign tech_posts = site.posts 
  | where_exp:"post","post.path contains '_posts/tech/'" 
  | sort: "date" 
  | reverse %}

<p>共有 {{ tech_posts | size }} 篇</p>

<ul>
{% for post in tech_posts limit:20 %}
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


[查看全部 →](/tech/)

---

## note

<p>共有 {{ site.note | size }} 篇</p>

{% assign notes = site.note | sort: "date" | reverse %}

<ul>
{% for post in notes limit:2 %}
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

[查看全部 →](/note/)

---

## 热门标签

{% assign tech_posts = site.posts | where_exp:"post","post.path contains '_posts/tech/'" %}
{% assign all_posts = tech_posts | concat: site.note %}

{% assign tags = "" | split: "" %}

{% for post in all_posts %}
  {% if post.tags %}
    {% assign tags = tags | concat: post.tags %}
  {% endif %}
{% endfor %}

{% assign sorted_tags = tags | uniq | sort %}

<div style="margin-bottom:20px;">
{% for tag in sorted_tags limit:5 %}
  <a href="/tag/#{{ tag }}" 
     style="margin-right:10px;padding:4px 8px;background:#f2f2f2;border-radius:5px;">
     #{{ tag }}
  </a>
{% endfor %}
</div>

## 联系我

- [bilibili](https://space.bilibili.com/3494372658121066)
- [Email](mailto:G114514g@yeah.net)
- [YouTube](https://youtube.com/@lm-xiao-fen)
