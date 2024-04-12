---
title: "Awards and Honors"
layout: textlay
sitemap: false
permalink: /awards and honors/
---

## Awards and Honors

<div class="jumbotron">
<ul>
{% for awards in site.data.awards %}

<li>{{ awards.name }}</li>

{% endfor %}
</ul>
</div>
