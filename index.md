---
layout: default
title: 首页
---

# 👋 欢迎访问我的博客

这里是我记录思考、模型构建与项目实践的地方。内容涵盖数据分析、建模、风控、系统设计等。

---

## 📄 最近文章

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>

---

## 📬 联系方式

- GitHub: [@wmding](https://github.com/wmding)
- Email: wmding@126.com