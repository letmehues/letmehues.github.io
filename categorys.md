---
layout: page
title: 分类
permalink: /categorys/
---


{% for cat in site.categories %} {{ cat[0] }} ({{ cat[1].size }}) {% endfor %}
{% for cat in site.categories %}
{{ cat[0] }}
{% for post in cat[1] %}
{{ post.date | date:"%Y-%m-%d" }} {{ post.title }}
{% endfor %} {% endfor %}
