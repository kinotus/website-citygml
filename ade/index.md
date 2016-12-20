---
layout: page
title:  Application Domain Extensions (ADE)
permalink: /ade/
---

- - -

* Table of Content
{:toc}

- - -

# Application Domain Extensions (ADE)
    
CityGML represents not only the graphical appearance of 3D city models but also the semantics associated with the city models.
For this, CityGML has a geometric model and a thematic model.
The thematic model of CityGML covers various classes like *buildings, relief, transportation, landuse, tunnels, bridges, vegetation, water bodies and city furniture.*
The objects which are not yet specifically modelled in CityGML can be represented using *generic objects and attributes*.
This is a semi structured extension mechanism without making any changes in the CityGML schema.
The generic extensions of CityGML are provided by the CityGML thematic module *Generics*.
But they have their own limitations, namely:

  * There is no formal specification of their names and data types.
  * Such CityGML files cannot be validated against the schema.
  * Name conflicts of the generic attributes and objects may occur.
  * Limited number of data types for generic attributes and objects.
  * Limits semantic and syntactic interoperability.


CityGML also has the concept of **ADE (Application Domain Extension)** to extend the schema with new classes and attributes which are not explicitly modelled in CityGML.
The difference between ADEs and generics is that an ADE is defined in an extra XSD (XML Schema Definition) file with its own namespace. 
This file has to explicitly import the XML Schema definition of the extended CityGML modules.
ADEs can be defined by information communities which are interested in specific application fields. 
ADEs are increasingly being used in creating application specific extensions like for energy modelling, modelling topographic data, indoor modelling, noise modelling, etc.
The advantage of using the ADE approach are:

  * The extensions are formally specified. 
  * This ensure semantic and syntactic interoperability for the exchange of application specific information.
  * Extended CityGML instance documents can be validated against the CityGML and the respective ADE schema. 
  * More than one ADE can be actively used in the same dataset.

- - -

# CityGML ADEs

{% assign ades = site.data.ade | bettersort: 'name' %}

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
    <td>{% if i.xmlschema == none %} <b>Not available</b> {% else %}<a href="{{ i.xmlschema }}">{{ i.name }} XSD</a>{% endif %}</td>
  </tr>  
  <tr>
    <td><b>UML Schema:</b></td>
    <td>{% if i.umlschema == none %} <b>Not available</b> {% else %}<a href="{{ i.umlschema }}">{{ i.name }} UML</a>{% endif %}</td>
  </tr>  
</table>
</div>
</div>

{% endfor %}

<!-- - - - 

# CityGML ADE Modelling -->

