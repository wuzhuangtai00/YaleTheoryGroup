---
title: "News"
layout: textlay
sitemap: false
permalink: https://www.cs.yale.edu/theory/news.html
---

## News

<div class="jumbotron">

{% for article in site.data.news %}
<h5>{{ article.date }}</h5>
<!-- <a href={{ article.link }}>{{ article.headline }}</a> -->
{% if article.link == null %}
{{article.headline}}
{% else %}
[{{ article.headline }}]({{ article.link }})
{% endif %}
{% endfor %}
</div>
