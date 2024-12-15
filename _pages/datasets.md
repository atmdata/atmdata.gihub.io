---
layout: basic
title: Datasets
permalink: /datasets/
---

<ul>
 {% for post in site.posts %}
     {% if post.tags[0] == "dataset" %}
     <li><span>{{ post.date | date: "%Y" }}</span>
     <i class="fas fa-angle-double-right" style="color: #aabcbc"></i>
     <a href="{{ post.url }}">{{ post.title }}</a> ({{ post.author }})</li>
     {% endif %}
 {% endfor %}
</ul>
