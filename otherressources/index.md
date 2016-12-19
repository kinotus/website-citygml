---
layout: page
title: Other useful CityGML ressources
permalink: /otherressources/
---

# Other useful CityGML ressources

{% assign ressources = site.data.ressources | sort: 'name' %}
{% for i in ressources %}
<div class="panel panel-default">
  <div class="panel-heading"><a href="{{ i.link }}">{{ i.name }}</a></div>
  <div class="panel-body">
    {{ i.info | markdownify | remove: '<p>' | remove: '</p>' }}  
  </div>
</div>
{% endfor %}

