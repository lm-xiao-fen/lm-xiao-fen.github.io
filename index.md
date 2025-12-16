---
layout: default
title: xf_blog
---
### [xf_blog](/)  

# Hi, I'm lm-xiao-fen

欢迎来到我的个人主页
这里记录我在 **Web 开发 / Cloudflare / GitHub / UP 主 / YouTuber** 方面的内容

[副站](https://lm-xiao-fen.github.io/my-web/index.html)    

---

## Blog  
{% for post in site.posts limit:5 %}
- **[{{ post.title }}]({{ post.url }})** 
  <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}   

---

## 联系我

- [bilibili](https://space.bilibili.com/3494372658121066)
- [email: G114514g@yeah.net](mailto:G114514g@yeah.net)
- [YouTube](https://youtube.com/@lm-xiao-fen)
- <a href="https://icp.we2050.com/id.php?keyword=20259950" target="_blank"> <img src="https://icp.we2050.com/logo.png" width="20" height="20" style="vertical-align: middle; margin-right: 5px;">团ICP备20259950号</a>
