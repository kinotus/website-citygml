---
layout: page
title:  Papers, videos and presentations about CityGML
permalink: /material/
---

# Papers, videos and presentations about CityGML

## Videos

{% assign videos = site.data.videos | sort: 'year' %}

{% for i in videos reversed %}

<div class="row">
  <div class="col-lg-3 col-md-4 col-sm-6">
    {% if i.img %}
      <a href="{{ i.link }}"><img class="img-responsive" src="/img/material/{{ i.img }}" alt="..."></a>
    {% else %}  
      <img class="img-responsive" src="http://placehold.it/350x150" alt="...">
    {% endif %}
  </div>
  <div class="col-lg-9 col-md-8 col-sm-6">
    <p><b>{{ i.title }}</b> ({{ i.year }}).<br></p>
    {% if i.info %}
      <p>{{ i.info }}</p>
    {% endif %}
  </div>
</div>
<br>

{% endfor %}

- - - 
  
## Scientific articles

{% assign articles = site.data.articles | sort: 'year' %}

{% for i in articles reversed %}

<div class="row">
  <div class="col-lg-3 col-md-4 col-sm-6">
    {% if i.img %}
      <a href="{{ i.DOI }}"><img class="img-responsive" src="/img/material/{{ i.img }}" alt="..."></a>
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
      <a href="{{ i.DOI }}">[DOI]</a>
    {% endif %}
    </p>
  </div>
</div>
<br>

{% endfor %}

- - -

## Presentations, keynotes, slides

todo