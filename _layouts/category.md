---
layout: default
title: 分类列表
---
<h2>{{ page.title }} </h2>
<ul>
{% for post in site.categories.[page.category] %}
<li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }} {{ post.url }}">{{ post.title }} </a>
</li>
{% endfor %}
</ul>
