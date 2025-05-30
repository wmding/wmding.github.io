---
layout: default
title: Tags
permalink: /tags/
---

<h2>🏷 All Tags</h2>
<ul>
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    <li>
      <a href="/tags/{{ tag[0] | slugify }}/">{{ tag[0] }} ({{ tag[1].size }})</a>
    </li>
  {% endfor %}
</ul>