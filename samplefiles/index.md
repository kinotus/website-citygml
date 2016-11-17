---
layout: page
title:  Sample CityGML files
permalink: /samplefiles/
---

# Sample CityGML files

{% assign ds = site.data.samplefiles | sort: 'year' %}

{% for i in ds %}

<div class="row">
  <div class="col-lg-3 col-md-4 col-sm-6">
    <img class="img-responsive" src="{{ i.image }}" alt="...">
  </div>
  <div class="col-lg-9 col-md-8 col-sm-6">
    <h4>{{ i.dataset }}</h4>
    <p><a href="{{ i.link }}">{{ i.link }}</a></p>
    {{ i.description | markdownify }}
    <p><i class="fa fa-copyright" aria-hidden="true"></i> {{ i.copyright | markdownify | remove: '<p>' | remove: '</p>' }}</p>
  </div>
</div>

{% endfor %}