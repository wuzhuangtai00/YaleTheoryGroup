---
title: "Students"
layout: gridlay
sitemap: false
permalink: https://www.cs.yale.edu/theory/students.html
---

<h5> Information on this page may be incomplete and needs to be updated </h5>

<div class='jumbotron'>
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-2">
<a href="{{member.homepage}}">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</a>
</div>
<div class="col-sm-4 col-xs-12">
<h4><a href="{{member.homepage}}">{{ member.name }}</h4>
<p><strong>Interest:</strong> {{member.interest}}</p>
<p><strong>Email:</strong> {{member.email}}</p>
</div>
<!-- </div> -->

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
</div>

