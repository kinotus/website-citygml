---
layout: page
title:  Sample CityGML files
permalink: /samplefiles/
---

# Sample CityGML files

{% assign ds = site.data.samplefiles | sort: 'year' %}

{% for i in ds %}

<div class="media">
  <div class="media-left">
    <img class="media-object" width="200px" src="{{ i.image }}" alt="...">
  </div>
  <div class="media-body">
    <h4 class="media-heading">{{ i.dataset }}</h4>
    <p><a href="{{ i.link }}">{{ i.link }}</a></p>
    {{ i.description | markdownify }}
    <p><i class="fa fa-copyright" aria-hidden="true"></i> {{ i.copyright | markdownify | remove: '<p>' | remove: '</p>' }}</p>
  </div>
</div>

{% endfor %}