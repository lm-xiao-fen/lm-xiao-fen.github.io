---
layout: home
title: xf_blog
---
### [xf_blog](/)　[副站](https://mikufans1.dpdns.org)　[友链](/feed-link)　[技术博客](/tech)　[随笔](/note)

# Hi, I am xiaofen

- 欢迎来到我的个人主页
- 这里记录我在 **Web 开发 / Cloudflare / GitHub** 方面的内容

---

## 技术博客
{% for post in site.posts limit:5 %}
  {% if post.path contains '_posts/tech/' %}
    ...
  {% endif %}
{% endfor %}

## 随记
{% for post in site.note limit:5 %}
  ...
{% endfor %}

---

## 联系我

- [bilibili](https://space.bilibili.com/3494372658121066)
- [Email](mailto:G114514g@yeah.net)
- [YouTube](https://youtube.com/@lm-xiao-fen)
