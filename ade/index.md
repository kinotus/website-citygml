---
layout: page
title:  Application Domain Extensions (ADE)
permalink: /ade/
---

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
The advantage of using the ADE approach are:

* The extensions are formally specified. 

* This ensure semantic and syntactic interoperability for the exchange of application specific information.

* Extended CityGML instance documents can be validated against the CityGML and the respective ADE schema. 

* ADEs can be defined by information communities which are interested in specific application fields. 
ADEs are increasingly being used in creating application specific extensions like for energy modelling, modelling topographic data, indoor modelling, noise modelling, etc.

* More than one ADE can be actively used in the same dataset.


## CityGML ADEs

### CityGML Noise ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Noise ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/)

* **UML Diagram:** [Noise ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/noise-ade/)

* **Documentation:**

### CityGML Robotics ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Robotics ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Robotics ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Energy ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Energy ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Energy ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML IMGeo ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [IMGeo ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [IMGeo ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Solar ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Solar ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Solar ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML GeoBIM ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [GeoBIM XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [GeoBIM UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML CAFM ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [CAFM ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [CAFM ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Hydro ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Hydro ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Hydro ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Utility Network ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Utility Network ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Utility Network ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Inclusive Routing ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Inclusive Routing ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Inclusive Routing ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Immovable Property Taxation ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Immovable Property Taxation ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Immovable Property Taxation ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**

### CityGML Time Dependent Variables ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** [Time Dependent Variables ADE XSD](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **UML Diagram:** [Time Dependent Variables ADE UML](http://schemas.opengis.net/citygml/examples/2.0/ade/robotics-ade/)

* **Documentation:**


### CityGML Terrain ADE

* **Description:** 

* **Version:**  

* **Status:** 

* **Contact Person:** 

* **Contact Organization:**

* **XML Schema:** Coming soon

* **UML Diagram:** Coming soon

* **Documentation:** 


## Modelling a CityGML ADE

