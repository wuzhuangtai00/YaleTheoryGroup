---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
---

## News

<div class="jumbotron">

{% for article in site.data.news %}
<b>{{ article.date }}</b>

<!-- <a href={{ article.link }}>{{ article.headline }}</a> -->
{% if article.link == null %}
{{article.headline}}
{% else %}
[{{ article.headline }}]({{ article.link }})
{% endif %}
{% endfor %}
</div>
