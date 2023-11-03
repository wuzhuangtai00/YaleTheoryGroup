---
title: "Faculty"
layout: gridlay
sitemap: false
permalink: https://www.cs.yale.edu/theory/faculty.html
---

{% for member in site.data.faculty %}

<div class="jumbotron">
<div class="row">
<div class="col-sm-4">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-8 col-xs-12">
<h3>{{ member.name }}</h3>
<p>{{ member.info }}</p>
<p><strong>Interest:</strong> {{member.interest}}</p>
<p><strong>Email:</strong> {{member.email}}</p>
<p><strong>Homepage:</strong> <a href="{{member.homepage}}">{{member.homepage}}</a></p>
</div>
</div>
</div>

{% endfor %}