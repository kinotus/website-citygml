---
layout: page
title:  Application Domain Extensions (ADE)
permalink: /ade/
---

- - -

* Table of Content
{:toc}

- - -
<div>
  <b><h2>Application Domain Extensions (ADEs)</h2></b><br/><br/>
</div>


<div class="container">
<div class="row">
<div class="col-md-7">
<p align="justify">
<font size="3">
CityGML is an XML based 3D data standard for the representation, storage and exchange of 3D city models. 
CityGML represents the geometry, graphical appearance and semantics associated with the 3D city models.
CityGML has a geometric model and a thematic model.
The thematic model of CityGML covers various classes like <i>buildings, relief, transportation, landuse, tunnels, bridges, vegetation, water bodies and city furniture.</i>
<br/>
<br/>
Sometimes, users may want to model objects and attributes of 3D city models which are not covered in the data model of CityGML.
CityGML has the concept of <i>ADEs (Application Domain Extensions)</i> to model user defined objects and attributes.
An ADE is defined in an extra XSD (XML Schema Definition) file with its own namespace. 
This file has to explicitly import the XML schema definition of the extended CityGML modules.
ADEs can be defined by information communities which are interested in specific application fields. 
ADEs are increasingly being used in creating application specific extensions like for energy modelling, modelling topographic data, indoor modelling, noise modelling, etc.
The advantage of using the ADE approach are:
<ul>
<li>The extensions are formally specified.</li>
<li>Semantic and syntactic interoperability for the exchange of application specific information.</li>
<li>Extended CityGML instance documents can be validated against the ADE schema. </li>
<li>More than one ADE can be actively used in the same dataset.</li>
<li>ADEs can have their own codelist. </li>
</ul>  
</font>
</p>
<p align="justify">
<font size="3">

Another approach is to use <i>Generic objects and attributes.</i>
This is a semi structured extension mechanism of adding application specific attributes and objects to city objects without making any changes in the CityGML schema.
The generic extensions of CityGML are provided by the CityGML thematic module <i>Generics</i>.
But they have their own limitations, namely:
<ul>
<li>There is no formal specification of the names and data types of generic attributes/objects.</li>
<li>CityGML datasets with generic atttributes/objects cannot be validated against the schema.</li>
<li>Name conflicts of the generic attributes and objects may occur.</li>
<li>Using Generics limits semantic and syntactic interoperability.</li>
</ul>
</font>
</p> 
<br /><br />
</div>

<div class="col-md-5">
<div>
     <br />
      <br />
      <br/>
      <br />
      <p align="center">
      <br/>
      <img src="ade.jpg" alt="" class="img-rounded pull-center" />
      <br/>
      <font size="4">
      CityGML ADE Modelling
    </font>
    </p>
    </div>
    <div>

    </div>
  </div>


 <div>
  <b><h2>CityGML ADEs</h2></b><br/><br/>
</div>

{% assign ades = site.data.ade | sort: 'name' %}

{% for i in ades %}

{% assign adeid = i.name | split: " " %}

<div class="panel panel-warning">
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href='#{{ adeid.first }}' class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        {{ i.name }}
      </a>
    </h4>
  </div>

<div id="{{ adeid.first }}" class="panel-collapse collapse">
<div class="panel-body">
<table class="table table-condensed table-hover table-responsive">
  <tr>
    <td><b>Description:</b></td>
    <td>{{ i.description }}</td>
  </tr>
  <tr>
    <td><b>ADE Version:</b></td>
    <td>{{ i.adeversion }}</td>
  </tr>
  <tr>
    <td><b>CityGML Version:</b></td>
    <td>{{ i.cityversion }}</td>
  </tr>  
  <tr>
    <td><b>Status:</b></td>
    <td>{{ i.status }}</td>
  </tr>    
  <tr>
    <td><b>Contact Organization:</b></td>
    <td>{{ i.contactorg }}</td>
  </tr>  
  <tr>
    <td><b>XML Schema:</b></td>
    <td>{% if i.xmlschema %} <a href="{{ i.xmlschema }}">{{ i.name }} XSD</a>{% endif %}</td>
  </tr>  
  <tr>
    <td><b>UML Schema:</b></td>
    <td>{% if i.umlschema %} <a href="{{ i.umlschema }}">{{ i.name }} UML</a>{% endif %}</td>
  </tr> 
  <tr>
    <td><b>Publication:</b></td>
    <td>{% if i.publication %} <a href="{{ i.publication }}">{{ i.name }} Publication</a>{% endif %}</td>
  </tr>  
</table>
</div>
</div>

{% endfor %}


<!-- - - - 

# CityGML ADE Modelling -->

