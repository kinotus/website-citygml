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


# CityGML ADEs

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Noise ADE
      </a>
    </h4>
  </div>

  <div id="saleitem" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Noise ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Noise ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem2" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Robotics ADE
      </a>
    </h4>
  </div>

  <div id="saleitem2" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Robotics ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Robotics ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

# CityGML ADE Modelling

