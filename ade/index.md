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

<table>
  <tr>
  <td width="500">
  <pre>
    

CityGML represents not only the graphical appearance of 3D city models but also the semantics associated with the city models.
For this, CityGML has a geometric model and a thematic model.
The thematic model of CityGML covers various classes like <i>buildings, relief, transportation, landuse, tunnels, bridges, vegetation, water bodies and city furniture.</i>
The objects which are not yet specifically modelled in CityGML can be represented using <i>generic objects and attributes.</i>
This is a semi structured extension mechanism without making any changes in the CityGML schema.
The generic extensions of CityGML are provided by the CityGML thematic module <i>Generics</i>.
But they have their own limitations, namely:

* There is no formal specification of their names and data types.

* Such CityGML files cannot be validated against the schema.

* Name conflicts of the generic attributes and objects may occur.

* Limited number of data types for generic attributes and objects.

* Limits semantic and syntactic interoperability.


CityGML also has the concept of <b>ADE (Application Domain Extension)</b> to extend the schema with new classes and attributes which are not explicitly modelled in CityGML.
The difference between ADEs and generics is that an ADE is defined in an extra XSD (XML Schema Definition) file with its own namespace. 
This file has to explicitly import the XML Schema definition of the extended CityGML modules.
ADEs can be defined by information communities which are interested in specific application fields. 
ADEs are increasingly being used in creating application specific extensions like for energy modelling, modelling topographic data, indoor modelling, noise modelling, etc.
The advantage of using the ADE approach are:

* The extensions are formally specified. 

* This ensure semantic and syntactic interoperability for the exchange of application specific information.

* Extended CityGML instance documents can be validated against the CityGML and the respective ADE schema. 

* More than one ADE can be actively used in the same dataset.

</pre>
</td>
<td width="200"></td>    
</tr>
</table>


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

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem3" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Energy ADE
      </a>
    </h4>
  </div>

  <div id="saleitem3" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Energy ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Energy ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem4" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Solar ADE
      </a>
    </h4>
  </div>

  <div id="saleitem4" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Solar ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Solar ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem5" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML GeoBIM ADE
      </a>
    </h4>
  </div>

  <div id="saleitem5" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> GeoBIM ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> GeoBIM ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem6" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML CAFM ADE
      </a>
    </h4>
  </div>

  <div id="saleitem6" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> CAFM ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> CAFM ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem7" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Hydro ADE
      </a>
    </h4>
  </div>

  <div id="saleitem7" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Hydro ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Hydro ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem8" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML UtilityNetwork ADE
      </a>
    </h4>
  </div>

  <div id="saleitem8" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> UtilityNetwork ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> UtilityNetwork ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem9" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Immovable Property Taxation ADE
      </a>
    </h4>
  </div>

  <div id="saleitem9" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Immovable Property Taxation ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Immovable Property Taxation ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem10" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Inclusive Routing ADE
      </a>
    </h4>
  </div>

  <div id="saleitem10" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Inclusive Routing ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Inclusive Routing ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

<div class="panel panel-warning">
 
    <h4 class="panel-title">
      <a data-toggle="collapse" data-parent="#panel" href="#saleitem11" class="panel-toggle">
        <span class="glyphicon glyphicon-folder-close"  id="icontoggle"></span>
        CityGML Time Dependent Variables ADE
      </a>
    </h4>
  </div>

  <div id="saleitem11" class="panel-collapse collapse">
     <div class="panel-body">
 <pre>        
* Description: 

* Version:  

* Status:

* Contact Person:

* Contact Organization:

* XML Schema: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Time Dependent Variables ADE XSD</a>

* UML Diagram: <a href="http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/" style="text-decoration:none"> Time Dependent Variables ADE UML</a>

* Documentation:
</pre>
</div>   
</div>

# CityGML ADE Modelling

