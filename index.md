---
layout: default
title: 首页
---

# 🏠 曲处同幽静

&gt; **柳暗花明又一村**

这里是 JC老师 的个人博客，记录美好生活，分享技术心得与读书感悟。

---

## 📝 最新文章

{% for post in site.posts limit:5 %}
**{{ post.date | date: "%Y年%m月%d日" }}**  
[{{ post.title }}]({{ post.url }})  
{% endfor %}

---

## 📚 文章分类

{% for category in site.categories %}
- **{{ category[0] }}** ({{ category[1].size }}篇)
{% endfor %}

---

## 🏷️ 热门标签

{% for tag in site.tags %}
- {{ tag[0] }} ({{ tag[1].size }})
{% endfor %}