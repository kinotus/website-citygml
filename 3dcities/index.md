---
layout: page
title:  Cities around the world with open datasets
permalink: /3dcities/
---

# Cities around the world with open CityGML datasets

{% assign ds = site.data.3dcities | sort: 'dataset' %}

<div class="table-responsive">

<table class="table table-striped">

  <tr class="info">
    <td>dataset</td>
    <td>country</td>
    <td>year</td>
    <td>Building LOD</td>
    <td>other classes</td>
    <td>textures</td>
    <td>acquisition</td>
    <td>CityGML version</td>
    <td>notes</td>
  </tr>

  {% for i in ds %}
    <tr>
      <td><a href="{{ i.link }}">{{ i.dataset }}</a></td>
      <td>{{ i.country }}</td>
      <td>{{ i.year }}</td>
      <td>{{ i.building_lod }}</td>
      <td>{{ i.classes }}</td>
      <td>{{ i.texture }}</td>
      <td>{{ i.acquisition | markdownify | remove: '<p>' | remove: '</p>' }}</td>
      <td>{{ i.version | markdownify | remove: '<p>' | remove: '</p>' }}</td>
      <td>{{ i.notes | markdownify | remove: '<p>' | remove: '</p>' }}</td>
    </tr>
  {% endfor %}

</table>
</div>

- - - 

<h1>Cities around the world with open 3D datasets <u>not</u> in CityGML</h1>

{% assign ds = site.data.3dcities_notcitygml | sort: 'dataset' %}

<div class="table-responsive">
<table class="table table-striped">

  <tr class="info">
    <td>dataset</td>
    <td>country</td>
    <td>year</td>
    <td>Building LOD</td>
    <td>other classes</td>
    <td>textures</td>
    <td>acquisition</td>
    <td>formats</td>
    <td>notes</td>
  </tr>

  {% for i in ds %}
    <tr>
      <td><a href="{{ i.link }}">{{ i.dataset }}</a></td>
      <td>{{ i.country }}</td>
      <td>{{ i.year }}</td>
      <td>{{ i.building_lod }}</td>
      <td>{{ i.classes }}</td>
      <td>{{ i.texture }}</td>
      <td>{{ i.acquisition }}</td>
      <td>{{ i.formats }}</td>
      <td>{{ i.notes | markdownify | remove: '<p>' | remove: '</p>' }}</td>
    </tr>
  {% endfor %}

</table>
</div> 

- - -

<h1>Open LiDAR datasets</h1>

Another potentially relevant list is the one of national lidar datasets on <a href="https://en.wikipedia.org/wiki/National_lidar_dataset">Wikipedia</a>. These datasets can be used as input to generate 3D city models. A possibility is to use the open-source software <a href="https://github.com/tudelft3d/3dfier">3dfier</a> developed at <a href="https://3d.bk.tudelft.nl/">TU Delft</a>, or <a href="{{ site.baseurl }}/software/#generators-of-3d-city-models-in-citygml">other CityGML software</a>.<br><br><br>