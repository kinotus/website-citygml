---
layout: page
title: Software
permalink: /software/
---

- - -

* Table of Content
{:toc}

- - -

{% assign software = site.data.software | sort: 'name' %}

## Viewers
{% for i in software %}
{% if i.category == 'viewer' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img src="/img/foss.png"> {% endif %}{% if i.starred %} <i class="fa fa-star"></i> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

## Generators of 3D city models in CityGML
{% for i in software %}
{% if i.category == 'generator' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img src="/img/foss.png"> {% endif %}{% if i.starred %} <i class="fa fa-star"></i> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

## Parsers and API for programmers
{% for i in software %}
{% if i.category == 'parser' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img src="/img/foss.png"> {% endif %}{% if i.starred %} <i class="fa fa-star"></i> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

## Validators of different aspects of CityGML
{% for i in software %}
{% if i.category == 'validator' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img src="/img/foss.png"> {% endif %}{% if i.starred %} <i class="fa fa-star"></i> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

## Storage in DBMS
{% for i in software %}
{% if i.category == 'storage' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img src="/img/foss.png"> {% endif %}{% if i.starred %} <i class="fa fa-star"></i> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

## Software that uses CityGML as input
{% for i in software %}
{% if i.category == 'applications' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img src="/img/foss.png"> {% endif %}{% if i.starred %} <i class="fa fa-star"></i> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}



