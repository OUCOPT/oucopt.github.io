---
title: "O2R Group News"
layout: textlay
excerpt: "O2R Group at OUC."
sitemap: false
permalink: /allnews.html
---

# 新闻动态

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}