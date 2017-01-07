---
layout: page
title: Other useful CityGML resources
permalink: /otherresources/
---

# Other useful CityGML resources


{% assign resources = site.data.resources | sort: 'name' %}
<div class="row">
{% for i in resources %}
  <div class="col-md-6 col-sm-12">
    <div class="panel panel-default">
      <div class="panel-heading"><a href="{{ i.link }}">{{ i.name }}</a></div>
      <div class="panel-body">
        {{ i.info | markdownify | remove: '<p>' | remove: '</p>' }}  
      </div>
    </div>
  </div>
{% endfor %}
</div>
