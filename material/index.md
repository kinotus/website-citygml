---
layout: page
title:  Papers, videos and presentations about CityGML
permalink: /material/
---


## Videos

  - [Webminar: How the OGC’s CityGML Standard Supports 3D Innovation for Business and Government](http://www.directionsmag.com/webinars/view/ogc-placeholder/216618)
  - [Course "100% CityGML", offered at TU Delft on 2011/03/14](http://collegerama.tudelft.nl/mediasite/SilverlightPlayer/Default.aspx?peid=7b440617cd1342b0b5b006fc0f6563ef1d)


## Presentations, keynotes, slides

  
## Scientific articles

{% assign articles = site.data.articles | sort: 'year' %}

{% for i in articles reversed %}

<div class="row">
  <div class="col-lg-3 col-md-4 col-sm-6">
    {% if i.img %}
      <a href="{{ i.DOI }}"><img class="img-responsive" src="/img/articles/{{ i.img }}" alt="..."></a>
    {% else %}  
      <img class="img-responsive" src="http://placehold.it/350x150" alt="...">
    {% endif %}
  </div>
  <div class="col-lg-9 col-md-8 col-sm-6">
    <p>
    <b>{{ i.title }}</b>
    ({{ i.year }}).
    {% for n in i.author %}
      {% if n.dropping-particle %}{{ n.dropping-particle }}{% endif %} {{ n.family}}, {{ n.given}}; 
    {% endfor %}
    <i>{{ i.container-title }}</i>,
    {% if i.volume %}{{ i.volume }}{% endif %}{% if i.issue %}({{ i.issue }}),{% endif %}
    {% if i.chapter-number %}chapter {{ i.chapter-number }},{% endif %}
    {% if i.page %}p.{{ i.page }}.{% endif %}
    {% if i.publisher %}{{ i.publisher }}.{% endif %}
    {% if i.DOI %}
      <a href="{{ i.DOI }}"><i class="fa fa-external-link"></i></a>
    {% endif %}
    </p>
  </div>
</div>
<br>

{% endfor %}
