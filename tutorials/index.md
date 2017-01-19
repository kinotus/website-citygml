---
layout: page
title: Tutorials
permalink: /tutorials/
---

# Tutorials

{% assign z = site.data.tutorials %}

{% for i in z %}

<div class="row">
  <div class="col-md-3 col-sm-6">
    {% if i.img %}
      <a href="{{ i.link }}"><img class="img-responsive" src="{{ i.img }}" alt="..."></a>
    {% else %}  
      <img class="img-responsive" src="http://placehold.it/350x150" alt="...">
    {% endif %}  
  </div>
  <div class="col-md-9 col-sm-6">
    <h4>{{ i.name | markdownify | remove: '<p>' | remove: '</p>' }}</h4>
    <p>{{ i.info | markdownify | remove: '<p>' | remove: '</p>' }}</p>
  </div>
</div>
<br>

{% endfor %}
  