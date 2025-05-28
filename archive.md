---
layout: default
title: 文章归档
permalink: /archive/
---

<h2>📂 所有文章归档</h2>
<ul>
  {% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}
  {% for year in posts_by_year %}
    <h3>{{ year.name }}</h3>
    <ul>
      {% for post in year.items %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          <small>({{ post.date | date: "%Y-%m-%d" }})</small>
        </li>
      {% endfor %}
    </ul>
  {% endfor %}
</ul>