---
layout: page
title: Software
permalink: /software/
---

We offer here a *curated* list of sofware that we believe are useful to practioners and researchers dealing with CityGML.
Most of the software are recent and well-maintained; if you believe your software should be there please advertise it on the google-group.

Free and open-source software are marked by <img height="15" src="/img/foss.svg">

- - -

* Table of Content
{:toc}

- - -

{% assign software = site.data.software | bettersort: 'name' %}

## Viewers
{% for i in software %}
{% if i.category contains 'viewer' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img height="15" src="/img/foss.svg"> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

- - -

## Generators of 3D city models in CityGML
{% for i in software %}
{% if i.category contains 'generator' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img height="15" src="/img/foss.svg"> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

- - -

## Parsers and API for programmers
{% for i in software %}
{% if i.category contains 'parser' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img height="15" src="/img/foss.svg"> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

- - -

## Validators of different aspects of CityGML
{% for i in software %}
{% if i.category contains 'validator' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img height="15" src="/img/foss.svg"> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

- - -

## Storage in DBMS
{% for i in software %}
{% if i.category contains 'storage' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img height="15" src="/img/foss.svg"> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}

- - -

## Software that uses CityGML as input 
{% for i in software %}
{% if i.category contains 'applications' %}
<p><a href="{{ i.webpage }}">{{ i.name }}</a> {% if i.foss == true %}<img height="15" src="/img/foss.svg"> {% endif %}<br/> {{ i.description }} </p>
{% endif %}
{% endfor %}



