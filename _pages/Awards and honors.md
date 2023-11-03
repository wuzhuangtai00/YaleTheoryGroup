---
title: "Awards and Honors"
layout: textlay
sitemap: false
permalink: https://www.cs.yale.edu/theory/Awards and honors.html
---

## Awards and Honors

<div class="jumbotron">
<ul>
{% for awards in site.data.awards %}

<li>{{ awards.name }}</li>

{% endfor %}
</ul>
</div>
