Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# The Construction Resources (CR) Ontology

## Metadata
* **IRI**
  * `http://w3id.org/cr`
* **Creators(s)**
  * [Jacopo Cassandro](https://orcid.org/0000-0002-1487-8178)
    [[ORCID]](https://orcid.org/0000-0002-1487-8178)
    (<jacopo.cassandro@polimi.it></a>) of [Politecnico di Milano](https://www.dabc.polimi.it/persona/jacopo-cassandro/)
* **Contributor(s)**
  * [Claudio Mirarchi](https://orcid.org/0000-0002-9288-8662)
    [[ORCID]](https://orcid.org/0000-0002-9288-8662)
    (<claudio.mirarchi@polimi.it></a>) of [Politecnico di Milano, Dipartimento ABC](https://www.dabc.polimi.it/persona/claudio-mirarchi/)
  * [Philipp Hagedorn](https://orcid.org/0000-0002-6249-243X)
    [[ORCID]](https://orcid.org/0000-0002-6249-243X)
    (<philipp.hagedorn-n6v@rub.de></a>) of [Ruhr University Bochum, Computing in Engineering](https://www.inf.bi.ruhr-uni-bochum.de/iib/lehrstuhl/mitarbeiter/philipp_hagedorn.html.en)
* **Created**
  * 2024-12-12
* **Version Information**
  * 0.1
* **Imports**
  * [http://w3id.org/ci](http://w3id.org/ci)
* **License &amp; Rights**
  * [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
  * &copy; 2024 by DABC, PoliMi
* **Source**
  * [https://linkedbuildingdata.net/ldac2024/files/papers/LDAC2024_Camera_8.pdf](https://linkedbuildingdata.net/ldac2024/files/papers/LDAC2024_Camera_8.pdf)
* **Ontology RDF**
  * RDF ([resources.ttl](turtle))
### Description
<p>The Construction Resources (CR) Ontology is based on concepts and principles . </p>

## Table of Contents
1. [Classes](#classes)
1. [Object Properties](#objectproperties)
1. [Datatype Properties](#datatypeproperties)
1. [Namespaces](#namespaces)
1. [Legend](#legend)


## Overview

**Figure 1:** Ontology overview
## Classes
[Assignment](#Assignment),
[Consumption](#Consumption),
[Cost item to geometry assignment](#Costitemtogeometryassignment),
[DimensionParameter](#DimensionParameter),
[Equipment resource](#Equipmentresource),
[Labour resource](#Labourresource),
[Material resource](#Materialresource),
[Parameter](#Parameter),
[PerformanceParameter](#PerformanceParameter),
[PhysicalParameter](#PhysicalParameter),
[Resource](#Resource),
[Resource to cost item assignment](#Resourcetocostitemassignment),
[Resource to geometry assignment](#Resourcetogeometryassignment),
[Resource to task assignment](#Resourcetotaskassignment),
[ResourceApplication](#ResourceApplication),
[Standard](#Standard),
[Task to geometry assignment](#Tasktogeometryassignment),
[object type](#objecttype),
### ResourceApplication
Property | Value
--- | ---
IRI | `https://dtc-ontology.cms.ed.tum.de/ontology#ResourceApplication`
Super-classes |[cr:ResourceToTaskAssignment](https://w3id.org/cr#ResourceToTaskAssignment) (c)<br />
### Assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Assignment`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[cr:TaskToGeometryAssignment](https://w3id.org/cr#TaskToGeometryAssignment) (c)<br />[cr:ResourceToCostItemAssignment](https://w3id.org/cr#ResourceToCostItemAssignment) (c)<br />[cr:ResourceToGeometryAssignment](https://w3id.org/cr#ResourceToGeometryAssignment) (c)<br />[cr:CostItemToGeometryAssignment](https://w3id.org/cr#CostItemToGeometryAssignment) (c)<br />[cr:ResourceToTaskAssignment](https://w3id.org/cr#ResourceToTaskAssignment) (c)<br />
In domain of |[cr:refCostItem](https://w3id.org/cr#refCostItem) (op)<br />[cr:refTask](https://w3id.org/cr#refTask) (op)<br />[cr:refResource](https://w3id.org/cr#refResource) (op)<br />[cr:refGeometry](https://w3id.org/cr#refGeometry) (op)<br />
### Consumption
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Consumption`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp) **max** 1<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op) **max** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />[cr:resourceConsumption](https://w3id.org/cr#resourceConsumption) (op) **max** 1 [cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp) **max** 1<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp) **max** 1<br />[cr:parameterType](https://w3id.org/cr#parameterType) (dp) **max** 1<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp) **max** 1<br />
In domain of |[cr:parameterType](https://w3id.org/cr#parameterType) (dp)<br />[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op)<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp)<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp)<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp)<br />
In range of |[cr:resourceConsumption](https://w3id.org/cr#resourceConsumption) (op)<br />
### Cost item to geometry assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#CostItemToGeometryAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct](http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct) (c)<br />[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [https://w3id.org/ci#ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />
### DimensionParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#DimensionParameter`
Super-classes |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
In range of |[cr:resourceDimensionParameter](https://w3id.org/cr#resourceDimensionParameter) (op)<br />
### Equipment resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#EquipmentResource`
Super-classes |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Restrictions |[cr:resourcePhysicalParameter](https://w3id.org/cr#resourcePhysicalParameter) (op) **max** 10 [cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />[cr:minimunLevelLabourResource](https://w3id.org/cr#minimunLevelLabourResource) (dp) **max** 1<br />[cr:accessory](https://w3id.org/cr#accessory) (dp) **exactly** 1<br />[cr:rent](https://w3id.org/cr#rent) (dp) **exactly** 1<br />[cr:material](https://w3id.org/cr#material) (dp) **exactly** 1<br />[cr:use](https://w3id.org/cr#use) (dp) **max** 5<br />[cr:resourcePerformanceParameter](https://w3id.org/cr#resourcePerformanceParameter) (op) **max** 10 [cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />[cr:resourceObjectStandard](https://w3id.org/cr#resourceObjectStandard) (op) **max** 1 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:resourceOtherStandard](https://w3id.org/cr#resourceOtherStandard) (op) **max** 5 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:resourceDimensionParameter](https://w3id.org/cr#resourceDimensionParameter) (op) **max** 10 [cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />[cr:function](https://w3id.org/cr#function) (dp) **max** 5<br />
In domain of |[cr:resourceDimensionParameter](https://w3id.org/cr#resourceDimensionParameter) (op)<br />[cr:function](https://w3id.org/cr#function) (dp)<br />[cr:resourceOtherStandard](https://w3id.org/cr#resourceOtherStandard) (op)<br />[cr:resourceObjectStandard](https://w3id.org/cr#resourceObjectStandard) (op)<br />[cr:rent](https://w3id.org/cr#rent) (dp)<br />[cr:cam](https://w3id.org/cr#cam) (dp)<br />[cr:material](https://w3id.org/cr#material) (dp)<br />[cr:resourceConsumption](https://w3id.org/cr#resourceConsumption) (op)<br />[cr:minimunLevelLabourResource](https://w3id.org/cr#minimunLevelLabourResource) (dp)<br />[cr:resourcePhysicalParameter](https://w3id.org/cr#resourcePhysicalParameter) (op)<br />[cr:resourcePerformanceParameter](https://w3id.org/cr#resourcePerformanceParameter) (op)<br />[cr:yield](https://w3id.org/cr#yield) (dp)<br />[cr:use](https://w3id.org/cr#use) (dp)<br />[cr:aspect](https://w3id.org/cr#aspect) (dp)<br />[cr:accessory](https://w3id.org/cr#accessory) (dp)<br />
### Labour resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#LabourResource`
Super-classes |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Restrictions |[cr:qualificationLevel](https://w3id.org/cr#qualificationLevel) (dp) **max** 1<br />
In domain of |[cr:qualificationLevel](https://w3id.org/cr#qualificationLevel) (dp)<br />
### Material resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#MaterialResource`
Super-classes |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Restrictions |[cr:use](https://w3id.org/cr#use) (dp) **max** 5<br />[cr:function](https://w3id.org/cr#function) (dp) **max** 5<br />[cr:furnishing](https://w3id.org/cr#furnishing) (dp) **max** 5<br />[cr:resourceOtherStandard](https://w3id.org/cr#resourceOtherStandard) (op) **max** 5 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:resourceObjectStandard](https://w3id.org/cr#resourceObjectStandard) (op) **max** 1 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:material](https://w3id.org/cr#material) (dp) **exactly** 1<br />[cr:finishing](https://w3id.org/cr#finishing) (dp) **max** 5<br />[cr:resourceDimensionParameter](https://w3id.org/cr#resourceDimensionParameter) (op) **max** 10 [cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />[cr:cam](https://w3id.org/cr#cam) (dp) **exactly** 1<br />[cr:resourcePhysicalParameter](https://w3id.org/cr#resourcePhysicalParameter) (op) **max** 10 [cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />[cr:resourcePerformanceParameter](https://w3id.org/cr#resourcePerformanceParameter) (op) **max** 10 [cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />
In domain of |[cr:furnishing](https://w3id.org/cr#furnishing) (dp)<br />[cr:function](https://w3id.org/cr#function) (dp)<br />[cr:resourceOtherStandard](https://w3id.org/cr#resourceOtherStandard) (op)<br />[cr:finishing](https://w3id.org/cr#finishing) (dp)<br />[cr:resourceObjectStandard](https://w3id.org/cr#resourceObjectStandard) (op)<br />[cr:resourcePhysicalParameter](https://w3id.org/cr#resourcePhysicalParameter) (op)<br />[cr:cam](https://w3id.org/cr#cam) (dp)<br />[cr:material](https://w3id.org/cr#material) (dp)<br />[cr:resourceConsumption](https://w3id.org/cr#resourceConsumption) (op)<br />[cr:use](https://w3id.org/cr#use) (dp)<br />[cr:aspect](https://w3id.org/cr#aspect) (dp)<br />[cr:yield](https://w3id.org/cr#yield) (dp)<br />[cr:resourcePerformanceParameter](https://w3id.org/cr#resourcePerformanceParameter) (op)<br />[cr:resourceDimensionParameter](https://w3id.org/cr#resourceDimensionParameter) (op)<br />
### object type
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ObjectType`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
### Parameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Parameter`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp) **max** 1<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp) **max** 1<br />[cr:resourceParameterStandard](https://w3id.org/cr#resourceParameterStandard) (op) **max** 1 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op) **max** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />[cr:parameterType](https://w3id.org/cr#parameterType) (dp) **max** 1<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp) **max** 1<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp) **max** 1<br />
Sub-classes |[cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />[cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />[cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />
In domain of |[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp)<br />[cr:resourceParameterStandard](https://w3id.org/cr#resourceParameterStandard) (op)<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp)<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp)<br />[cr:parameterType](https://w3id.org/cr#parameterType) (dp)<br />[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op)<br />
### PerformanceParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#PerformanceParameter`
Super-classes |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
In range of |[cr:resourcePerformanceParameter](https://w3id.org/cr#resourcePerformanceParameter) (op)<br />
### PhysicalParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#PhysicalParameter`
Super-classes |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
In range of |[cr:resourcePhysicalParameter](https://w3id.org/cr#resourcePhysicalParameter) (op)<br />
### Resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Resource`
Description | <p>This class is used for providing information about a construction resource.</p>
Restrictions |[cr:descriptionGeneral](https://w3id.org/cr#descriptionGeneral) (dp) **exactly** 1<br />[cr:law](https://w3id.org/cr#law) (dp) **max** 10<br />[cr:code](https://w3id.org/cr#code) (dp) **exactly** 1<br />[cr:category](https://w3id.org/cr#category) (dp) **exactly** 1<br />[cr:quantityUnitOfMeasure](https://w3id.org/cr#quantityUnitOfMeasure) (dp) **exactly** 1<br />[cr:gender](https://w3id.org/cr#gender) (dp) **exactly** 1<br />[cr:object](https://w3id.org/cr#object) (dp) **exactly** 1<br />[cr:aspect](https://w3id.org/cr#aspect) (dp) **max** 5<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op) **exactly** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />[cr:family](https://w3id.org/cr#family) (dp) **exactly** 1<br />[cr:type](https://w3id.org/cr#type) (dp) **max** 1<br />[cr:keywords](https://w3id.org/cr#keywords) (dp) **max** 10<br />[cr:descriptionDetail](https://w3id.org/cr#descriptionDetail) (dp) **max** 1<br />
Sub-classes |[cr:LabourResource](https://w3id.org/cr#LabourResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
In domain of |[cr:object](https://w3id.org/cr#object) (dp)<br />[cr:descriptionDetail](https://w3id.org/cr#descriptionDetail) (dp)<br />[cr:techSpecs](https://w3id.org/cr#techSpecs) (dp)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op)<br />[cr:keywords](https://w3id.org/cr#keywords) (dp)<br />[cr:escluded](https://w3id.org/cr#escluded) (dp)<br />[cr:category](https://w3id.org/cr#category) (dp)<br />[cr:subRecourceOf](https://w3id.org/cr#subRecourceOf)<br />[cr:quantityUnitOfMeasure](https://w3id.org/cr#quantityUnitOfMeasure) (dp)<br />[cr:measurementRules](https://w3id.org/cr#measurementRules) (dp)<br />[cr:omniclass](https://w3id.org/cr#omniclass) (dp)<br />[cr:uniformat](https://w3id.org/cr#uniformat) (dp)<br />[cr:uniclass](https://w3id.org/cr#uniclass) (dp)<br />[cr:included](https://w3id.org/cr#included) (dp)<br />[cr:code](https://w3id.org/cr#code) (dp)<br />[cr:family](https://w3id.org/cr#family) (dp)<br />[cr:law](https://w3id.org/cr#law) (dp)<br />[cr:descriptionGeneral](https://w3id.org/cr#descriptionGeneral) (dp)<br />[cr:hasSubResource](https://w3id.org/cr#hasSubResource)<br />[cr:gender](https://w3id.org/cr#gender) (dp)<br />[cr:type](https://w3id.org/cr#type) (dp)<br />
In range of |[cr:hasSubResource](https://w3id.org/cr#hasSubResource)<br />[cr:subRecourceOf](https://w3id.org/cr#subRecourceOf)<br />[cr:refResource](https://w3id.org/cr#refResource) (op)<br />
### Resource to cost item assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ResourceToCostItemAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [https://w3id.org/ci#ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />[cr:refResource](https://w3id.org/cr#refResource) (op) **some** [cr:Resource](https://w3id.org/cr#Resource) (c)<br />
### Resource to geometry assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ResourceToGeometryAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refResource](https://w3id.org/cr#refResource) (op) **some** [cr:Resource](https://w3id.org/cr#Resource) (c)<br />[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct](http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct) (c)<br />
### Resource to task assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ResourceToTaskAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refResource](https://w3id.org/cr#refResource) (op) **some** [cr:Resource](https://w3id.org/cr#Resource) (c)<br />[cr:refTask](https://w3id.org/cr#refTask) (op) **some** [dtc:Task](https://dtc-ontology.cms.ed.tum.de/ontology/Task) (c)<br />
Sub-classes |[https://dtc-ontology.cms.ed.tum.de/ontology#ResourceApplication](https://dtc-ontology.cms.ed.tum.de/ontology#ResourceApplication) (c)<br />
### Standard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Standard`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:standardYear](https://w3id.org/cr#standardYear) (dp) **max** 1<br />[cr:standardNumber](https://w3id.org/cr#standardNumber) (dp) **max** 1<br />[cr:standardBody](https://w3id.org/cr#standardBody) (dp) **max** 1<br />[cr:standardPart](https://w3id.org/cr#standardPart) (dp) **max** 1<br />
In domain of |[cr:standardBody](https://w3id.org/cr#standardBody) (dp)<br />[cr:standardPart](https://w3id.org/cr#standardPart) (dp)<br />[cr:standardNumber](https://w3id.org/cr#standardNumber) (dp)<br />[cr:standardYear](https://w3id.org/cr#standardYear) (dp)<br />
In range of |[cr:resourceParameterStandard](https://w3id.org/cr#resourceParameterStandard) (op)<br />[cr:resourceObjectStandard](https://w3id.org/cr#resourceObjectStandard) (op)<br />[cr:resourceOtherStandard](https://w3id.org/cr#resourceOtherStandard) (op)<br />
### Task to geometry assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#TaskToGeometryAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct](http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct) (c)<br />[cr:refTask](https://w3id.org/cr#refTask) (op) **some** [dtc:Task](https://dtc-ontology.cms.ed.tum.de/ontology/Task) (c)<br />

## Object Properties
[hasUnit](#hasUnit),
[ref](#ref),
[ref cost item](#refcostitem),
[ref geometry](#refgeometry),
[ref resource](#refresource),
[ref task](#reftask),
[resourceConsumption](#resourceConsumption),
[resourceDimensionParameter](#resourceDimensionParameter),
[resourceObjectStandard](#resourceObjectStandard),
[resourceOtherStandard](#resourceOtherStandard),
[resourceParameterStandard](#resourceParameterStandard),
[resourcePerformanceParameter](#resourcePerformanceParameter),
[resourcePhysicalParameter](#resourcePhysicalParameter),
[](hasUnit)
### hasUnit
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasUnit`
Domain(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:Resource](https://w3id.org/cr#Resource) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />
[](ref)
### ref
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ref`
[](refcostitem)
### ref cost item
Property | Value
--- | ---
IRI | `https://w3id.org/cr#refCostItem`
Super-properties |[cr:ref](https://w3id.org/cr#ref) (op)<br />
Domain(s) |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Range(s) |[https://w3id.org/ci#ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />
[](refgeometry)
### ref geometry
Property | Value
--- | ---
IRI | `https://w3id.org/cr#refGeometry`
Super-properties |[cr:ref](https://w3id.org/cr#ref) (op)<br />
Domain(s) |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Range(s) |[http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct](http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct) (c)<br />
[](refresource)
### ref resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#refResource`
Super-properties |[cr:ref](https://w3id.org/cr#ref) (op)<br />
Domain(s) |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Range(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
[](reftask)
### ref task
Property | Value
--- | ---
IRI | `https://w3id.org/cr#refTask`
Super-properties |[cr:ref](https://w3id.org/cr#ref) (op)<br />
Domain(s) |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Range(s) |[https://dtc-ontology.cms.ed.tum.de/ontology#Task](https://dtc-ontology.cms.ed.tum.de/ontology#Task) (c)<br />
[](resourceConsumption)
### resourceConsumption
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourceConsumption`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
[](resourceDimensionParameter)
### resourceDimensionParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourceDimensionParameter`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />
[](resourceObjectStandard)
### resourceObjectStandard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourceObjectStandard`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
[](resourceOtherStandard)
### resourceOtherStandard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourceOtherStandard`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
[](resourceParameterStandard)
### resourceParameterStandard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourceParameterStandard`
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
[](resourcePerformanceParameter)
### resourcePerformanceParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourcePerformanceParameter`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />
[](resourcePhysicalParameter)
### resourcePhysicalParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#resourcePhysicalParameter`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />

## Datatype Properties
[accessory](#accessory),
[aspect](#aspect),
[cam](#cam),
[category](#category),
[code](#code),
[descriptionDetail](#descriptionDetail),
[descriptionGeneral](#descriptionGeneral),
[escluded](#escluded),
[family](#family),
[finishing](#finishing),
[function](#function),
[furnishing](#furnishing),
[gender](#gender),
[included](#included),
[keywords](#keywords),
[law](#law),
[material](#material),
[measurement rules](#measurementrules),
[minimunLevelLabourResource](#minimunLevelLabourResource),
[object](#object),
[omniclass](#omniclass),
[parameterSymbol1](#parameterSymbol1),
[parameterSymbol2](#parameterSymbol2),
[parameterType](#parameterType),
[parameterValue1](#parameterValue1),
[parameterValue2](#parameterValue2),
[qualificationLevel](#qualificationLevel),
[quantityUnitOfMeasure](#quantityUnitOfMeasure),
[rent](#rent),
[standardBody](#standardBody),
[standardNumber](#standardNumber),
[standardPart](#standardPart),
[standardYear](#standardYear),
[tech specs](#techspecs),
[type](#type),
[uniclass](#uniclass),
[uniformat](#uniformat),
[use](#use),
[yield](#yield),
[](accessory)
### accessory
Property | Value
--- | ---
IRI | `https://w3id.org/cr#accessory`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />
[](aspect)
### aspect
Property | Value
--- | ---
IRI | `https://w3id.org/cr#aspect`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](cam)
### cam
Property | Value
--- | ---
IRI | `https://w3id.org/cr#cam`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />
[](category)
### category
Property | Value
--- | ---
IRI | `https://w3id.org/cr#category`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](code)
### code
Property | Value
--- | ---
IRI | `https://w3id.org/cr#code`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](descriptionDetail)
### descriptionDetail
Property | Value
--- | ---
IRI | `https://w3id.org/cr#descriptionDetail`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](descriptionGeneral)
### descriptionGeneral
Property | Value
--- | ---
IRI | `https://w3id.org/cr#descriptionGeneral`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](escluded)
### escluded
Property | Value
--- | ---
IRI | `https://w3id.org/cr#escluded`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](family)
### family
Property | Value
--- | ---
IRI | `https://w3id.org/cr#family`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](finishing)
### finishing
Property | Value
--- | ---
IRI | `https://w3id.org/cr#finishing`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](function)
### function
Property | Value
--- | ---
IRI | `https://w3id.org/cr#function`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](furnishing)
### furnishing
Property | Value
--- | ---
IRI | `https://w3id.org/cr#furnishing`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](gender)
### gender
Property | Value
--- | ---
IRI | `https://w3id.org/cr#gender`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](included)
### included
Property | Value
--- | ---
IRI | `https://w3id.org/cr#included`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](keywords)
### keywords
Property | Value
--- | ---
IRI | `https://w3id.org/cr#keywords`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](law)
### law
Property | Value
--- | ---
IRI | `https://w3id.org/cr#law`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](material)
### material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#material`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](measurementrules)
### measurement rules
Property | Value
--- | ---
IRI | `https://w3id.org/cr#measurementRules`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](minimunLevelLabourResource)
### minimunLevelLabourResource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#minimunLevelLabourResource`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](object)
### object
Property | Value
--- | ---
IRI | `https://w3id.org/cr#object`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](omniclass)
### omniclass
Property | Value
--- | ---
IRI | `https://w3id.org/cr#omniclass`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterSymbol1)
### parameterSymbol1
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterSymbol1`
Domain(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterSymbol2)
### parameterSymbol2
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterSymbol2`
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterType)
### parameterType
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterType`
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterValue1)
### parameterValue1
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterValue1`
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](parameterValue2)
### parameterValue2
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterValue2`
Domain(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](qualificationLevel)
### qualificationLevel
Property | Value
--- | ---
IRI | `https://w3id.org/cr#qualificationLevel`
Domain(s) |[cr:LabourResource](https://w3id.org/cr#LabourResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](quantityUnitOfMeasure)
### quantityUnitOfMeasure
Property | Value
--- | ---
IRI | `https://w3id.org/cr#quantityUnitOfMeasure`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](rent)
### rent
Property | Value
--- | ---
IRI | `https://w3id.org/cr#rent`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />
[](standardBody)
### standardBody
Property | Value
--- | ---
IRI | `https://w3id.org/cr#standardBody`
Domain(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](standardNumber)
### standardNumber
Property | Value
--- | ---
IRI | `https://w3id.org/cr#standardNumber`
Domain(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](standardPart)
### standardPart
Property | Value
--- | ---
IRI | `https://w3id.org/cr#standardPart`
Domain(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](standardYear)
### standardYear
Property | Value
--- | ---
IRI | `https://w3id.org/cr#standardYear`
Domain(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](techspecs)
### tech specs
Property | Value
--- | ---
IRI | `https://w3id.org/cr#techSpecs`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](type)
### type
Property | Value
--- | ---
IRI | `https://w3id.org/cr#type`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](uniclass)
### uniclass
Property | Value
--- | ---
IRI | `https://w3id.org/cr#uniclass`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](uniformat)
### uniformat
Property | Value
--- | ---
IRI | `https://w3id.org/cr#uniformat`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](use)
### use
Property | Value
--- | ---
IRI | `https://w3id.org/cr#use`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](yield)
### yield
Property | Value
--- | ---
IRI | `https://w3id.org/cr#yield`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />

## Named Individuals
## Namespaces
* **cr**
  * `https://w3id.org/cr#`
* **dc**
  * `http://purl.org/dc/terms/`
* **dtc**
  * `https://dtc-ontology.cms.ed.tum.de/ontology/`
* **owl**
  * `http://www.w3.org/2002/07/owl#`
* **prov**
  * `http://www.w3.org/ns/prov#`
* **qudt**
  * `http://qudt.org/schema/qudt/`
* **rdf**
  * `http://www.w3.org/1999/02/22-rdf-syntax-ns#`
* **rdfs**
  * `http://www.w3.org/2000/01/rdf-schema#`
* **sdo**
  * `https://schema.org/`
* **skos**
  * `http://www.w3.org/2004/02/skos/core#`
* **vann**
  * `http://purl.org/vocab/vann/`
* **vs**
  * `http://www.w3.org/2003/06/sw-vocab-status/ns#`
* **xml**
  * `http://www.w3.org/XML/1998/namespace`
* **xsd**
  * `http://www.w3.org/2001/XMLSchema#`

## Legend
* Classes: c
* Object Properties: op
* Functional Properties: fp
* Data Properties: dp
* Annotation Properties: dp
* Properties: p
* Named Individuals: ni