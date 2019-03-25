---
layout: page
title: 标签
permalink: /tags/
---


{% for tag in site.tags %} {{ tag[0] }} {% endfor %}
{% for tag in site.tags %}
{{ tag[0] }}
{% for post in tag[1] %}
{{ post.date | date:"%Y-%m-%d" }} {{ post.title }}
{% endfor %} {% endfor %}
<script src="/js/jquery.tagcloud.js" type="text/javascript" charset="utf-8"></script> <script language="javascript"> $.fn.tagcloud.defaults = { size: {start: 1, end: 2, unit: 'em'}, color: {start: '#ada8b5', end: '#000000'} }; $(function () { $('#tag_cloud a').tagcloud(); }); </script>
