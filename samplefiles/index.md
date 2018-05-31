---
layout: page
title:  Sample CityGML files
permalink: /samplefiles/
---

# Example files for specific CityGML classes

<div class="row">
  <div class="col-md-4 col-sm-12">
    <div class="list-group">
      <a href="building" class="list-group-item list-group-item-info text-center">Building</a>
      <a href="terrain" class="list-group-item list-group-item-info text-center">Terrain</a>
<!--       <a href="landuse" class="list-group-item list-group-item-info text-center">Land Use</a> -->
      <a href="geomprimitives" class="list-group-item list-group-item-info text-center">3D geometric primitives</a>
    </div>
  </div>
</div>


- - - 

# Sample CityGML files

{% assign ds = site.data.samplefiles | sort: 'year' %}

{% for i in ds reversed %}

<div class="row">
  <div class="col-lg-3 col-md-4 col-sm-6">
    <img class="img-responsive" src="{{ i.image }}" alt="...">
  </div>
  <div class="col-lg-9 col-md-8 col-sm-6">
    <h4>{{ i.dataset }}</h4>
    <p><a href="{{ i.link }}">{{ i.link }}</a></p>
    {{ i.description | markdownify | remove: '<p>' | remove: '</p>' }}
    {% if i.copyright %}
    <p><i class="fa fa-copyright" aria-hidden="true"></i> {{ i.copyright | markdownify | remove: '<p>' | remove: '</p>' }}</p>
    {% endif %}
  </div>
</div>
<br>

{% endfor %}