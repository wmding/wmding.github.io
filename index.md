# 👋 欢迎来到我的主页

<div style="text-align:center">
  <img src="/assets/avatar.jpg" width="150" style="border-radius:50%">
  <p>数据建模 | 金融风控 | 系统工程</p>
</div>

---

## 📌 最新文章

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}