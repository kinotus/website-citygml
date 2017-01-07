---
layout: page
title:  CityGML Buildings
permalink: /samplefiles/building/
---

# How to represent a Building in CityGML, some examples

{% assign ds = site.data.classes.building %}

{% for i in ds %}

<div class="row">
  <div class="col-md-2 col-sm-6">
    <img class="img-responsive" src="{{ i.dataset }}.jpg" alt="...">
    <!-- <img class="img-responsive" src="{{ i.image }}" alt="..."> -->
  </div>
  <div class="col-md-10 col-sm-6">
    <h4>{{ i.description | markdownify | remove: '<p>' | remove: '</p>' }}</h4>
    <p>{{ i.info | markdownify | remove: '<p>' | remove: '</p>' }}</p>
    <p><i class="fa fa-download" aria-hidden="true"></i> <a href="{{ i.dataset }}.gml">{{ i.dataset }}.gml</a></p>
  </div>
</div>
<br>

{% endfor %}