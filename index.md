---
layout: home
title: xf_blog
permalink: /
---
### [xf_blog](/)&emsp;[副站](https://mikufans1.dpdns.org)&emsp;[友链](/feed-link/)&emsp;[归档](/archive/)&emsp;[标签](/tag/)&emsp;[分类](/classify/)

# Hi, I am xiaofen

> 欢迎来到我的个人主页
>
> 这里记录我在 **开发 / 生活** 方面的内容

---
## 近期更新

{% assign tech_posts = site.posts 
  | where_exp:"post","post.path contains '_posts/tech/'" 
  | sort: "date" 
  | reverse %}

<ul>
{% for post in tech_posts limit:2 %}
  <li style="margin-bottom:6px;">
    <span style="color:#8b949e; font-size:13px;">
      {{ post.date | date: "%Y-%m-%d" }}
    </span>
    <a href="{{ post.url }}" style="margin-left:6px;">
      {{ post.title }}
    </a>
    <span>
      tech
    </span>
  </li>
{% endfor %}
</ul>

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
  <span>
    note
  </span>
</li>
{% endfor %}
</ul>

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

  </ul>
</div>

## 社交的

[bilibili](https://space.bilibili.com/3494372658121066)&ensp;[Email](mailto:G114514g@yeah.net)&ensp;[YouTube](https://youtube.com/@lm-xiao-fen)&ensp;[rss](/feed.xml)