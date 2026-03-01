---
layout: home
title: xf_blog
---
### [xf_blog](/)　[副站](https://mikufans1.dpdns.org)　[友链](/feed-link)　[技术博客](/tech)　[随笔](/note)

# Hi, I am xiaofen

- 欢迎来到我的个人主页
- 这里记录我在 **Web 开发 / Cloudflare / GitHub** 方面的内容

---

{% assign tech_posts = site.posts | where_exp:"post","post.path contains '_posts/tech/'" %}

## 🛠 技术博客

<p>共有 {{ tech_posts | size }} 篇</p>

<ul>
{% for post in tech_posts limit:5 %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span>{{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>

<p><a href="/tech/">查看全部 →</a></p>

---

## 📝 随记

<p>共有 {{ site.note | size }} 篇</p>

<ul>
{% for post in site.note limit:5 %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

<p><a href="/note/">查看全部 →</a></p>

---

## 联系我

- [bilibili](https://space.bilibili.com/3494372658121066)
- [Email](mailto:G114514g@yeah.net)
- [YouTube](https://youtube.com/@lm-xiao-fen)
