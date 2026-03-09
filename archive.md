---
layout: default
title: 归档
permalink: /archive/
---

# 归档

<input id="searchInput" type="text" placeholder="搜索文章..." style="width:100%;padding:8px;margin-bottom:20px;">

<ul id="postList">
{% assign tech_posts = site.posts | where_exp:"post","post.path contains '_posts/tech/'" %}
{% assign all_posts = tech_posts | concat: site.note | sort:"date" | reverse %}

{% for post in all_posts %}
<li class="post-item">
  <span style="color:gray;">{{ post.date | date: "%Y-%m-%d" }}</span>
  <a href="{{ post.url }}">{{ post.title }}</a>
</li>
{% endfor %}

</ul>

<script>
const input = document.getElementById("searchInput");
const items = document.querySelectorAll(".post-item");

input.addEventListener("keyup", function() {
  const keyword = input.value.toLowerCase();

  items.forEach(item => {
    const text = item.innerText.toLowerCase();
    item.style.display = text.includes(keyword) ? "" : "none";
  });
});
</script>
