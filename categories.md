---
layout: default
title: Categories
permalink: /categories/
---

<h2>📂 All Categories</h2>
<ul>
  {% assign sorted_categories = site.categories | sort %}
  {% for category in sorted_categories %}
    <li>
      <a href="/categories/{{ category[0] | slugify }}/">{{ category[0] }} ({{ category[1].size }})</a>
    </li>
  {% endfor %}
</ul>