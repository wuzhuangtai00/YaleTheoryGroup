---
title: "Team"
layout: default
sitemap: false
permalink: /team/
---

## Team

**We are looking for new team members** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

<style>
  .flex-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }

  .flex-item {
    flex: 0 0 calc(33.3333% - 20px);
    margin: 10px;
    box-sizing: border-box;
  }
</style>

<div class="flex-container">

{% for member in site.data.pi %}
<div>
    <h4>{{ member.name }}</h4>
    <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" alt="{{ member.name }}">
</div>
{% endfor %}


</div>
