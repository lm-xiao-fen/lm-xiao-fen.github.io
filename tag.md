---
layout: page
title: 标签云
permalink: /tag/
---
# 全部标签

<div class="tag-cloud">
  {% assign tags = site.tags | sort %}
  {% for tag in tags %}
    <a href="/tag/{{ tag[0] | slugify }}" style="font-size: {{ tag[1] | size | times: 2 | plus: 12 }}px;">
      {{ tag[0] }} ({{ tag[1] | size }})
    </a>
  {% endfor %}
</div>
