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
[Family](#Family),
[Family of equipment](#Familyofequipment),
[Family of labour](#Familyoflabour),
[Family of material](#Familyofmaterial),
[Finishing](#Finishing),
[Function](#Function),
[Function of equipment](#Functionofequipment),
[Function of material](#Functionofmaterial),
[Furnishing](#Furnishing),
[Gender](#Gender),
[Labour resource](#Labourresource),
[Material](#Material),
[Material resource](#Materialresource),
[Object of equipment](#Objectofequipment),
[Object of labour](#Objectoflabour),
[Object of material](#Objectofmaterial),
[Parameter](#Parameter),
[PerformanceParameter](#PerformanceParameter),
[PhysicalParameter](#PhysicalParameter),
[QualificationLevel](#QualificationLevel),
[Resource](#Resource),
[Resource to cost item assignment](#Resourcetocostitemassignment),
[Resource to task assignment](#Resourcetotaskassignment),
[ResourceApplication](#ResourceApplication),
[Standard](#Standard),
[Task to geometry assignment](#Tasktogeometryassignment),
[Type](#Type),
[Type of equipment](#Typeofequipment),
[Type of labour](#Typeoflabour),
[Type of material](#Typeofmaterial),
[Use](#Use),
[Use of equipment](#Useofequipment),
[Use of material](#Useofmaterial),
[oObject](#oObject),
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
Sub-classes |[cr:CostItemToGeometryAssignment](https://w3id.org/cr#CostItemToGeometryAssignment) (c)<br />[cr:ResourceToCostItemAssignment](https://w3id.org/cr#ResourceToCostItemAssignment) (c)<br />[cr:TaskToGeometryAssignment](https://w3id.org/cr#TaskToGeometryAssignment) (c)<br />[cr:ResourceToTaskAssignment](https://w3id.org/cr#ResourceToTaskAssignment) (c)<br />
In domain of |[cr:refCostItem](https://w3id.org/cr#refCostItem) (op)<br />[cr:refTask](https://w3id.org/cr#refTask) (op)<br />[cr:refGeometry](https://w3id.org/cr#refGeometry) (op)<br />[cr:refResource](https://w3id.org/cr#refResource) (op)<br />
### Consumption
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Consumption`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:parameterType](https://w3id.org/cr#parameterType) (dp) **max** 1<br />[cr:hasConsumption](https://w3id.org/cr#hasConsumption) (op) **max** 1 [cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op) **max** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp) **max** 1<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp) **max** 1<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp) **max** 1<br />[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp) **max** 1<br />
In domain of |[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp)<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp)<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp)<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp)<br />[cr:parameterType](https://w3id.org/cr#parameterType) (dp)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op)<br />
In range of |[cr:hasConsumption](https://w3id.org/cr#hasConsumption) (op)<br />
### Cost item to geometry assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#CostItemToGeometryAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [ci:ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct](http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct) (c)<br />
### DimensionParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#DimensionParameter`
Super-classes |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
In range of |[cr:hasDimensionParameter](https://w3id.org/cr#hasDimensionParameter) (op)<br />
### Equipment resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#EquipmentResource`
Super-classes |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Restrictions |[cr:rent](https://w3id.org/cr#rent) (dp) **exactly** 1<br />[cr:hasObject](https://w3id.org/cr#hasObject) (op) **exactly** 1 [cr:ObjectOfEquipment](https://w3id.org/cr#ObjectOfEquipment) (c)<br />[cr:hasFunction](https://w3id.org/cr#hasFunction) (op) **max** 5 [cr:FunctionOfEquipment](https://w3id.org/cr#FunctionOfEquipment) (c)<br />[cr:hasMaterial](https://w3id.org/cr#hasMaterial) (op) **exactly** 1 [cr:Material](https://w3id.org/cr#Material) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfEquipment](https://w3id.org/cterm#CategoryOfEquipment) (c)<br />[cr:accessory](https://w3id.org/cr#accessory) (dp) **exactly** 1<br />[cr:hasUse](https://w3id.org/cr#hasUse) (op) **max** 5 [cr:Use](https://w3id.org/cr#Use) (c)<br />[cr:hasOtherStandard](https://w3id.org/cr#hasOtherStandard) (op) **max** 5 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:hasFamily](https://w3id.org/cr#hasFamily) (op) **exactly** 1 [cr:FamilyOfEquipment](https://w3id.org/cr#FamilyOfEquipment) (c)<br />[cterm:hasAspect](https://w3id.org/cterm#hasAspect) **max** 5 [cterm:AspectOfEquipment](https://w3id.org/cterm#AspectOfEquipment) (c)<br />[cr:minimunLevelLabourResource](https://w3id.org/cr#minimunLevelLabourResource) (dp) **max** 1<br />[cr:hasPhysicalParameter](https://w3id.org/cr#hasPhysicalParameter) (op) **max** 10 [cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />[cr:hasDimensionParameter](https://w3id.org/cr#hasDimensionParameter) (op) **max** 10 [cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />[cr:hasObjectStandard](https://w3id.org/cr#hasObjectStandard) (op) **max** 1 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:hasPerformanceParameter](https://w3id.org/cr#hasPerformanceParameter) (op) **max** 10 [cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />
In domain of |[cr:hasConsumption](https://w3id.org/cr#hasConsumption) (op)<br />[cr:hasObjectStandard](https://w3id.org/cr#hasObjectStandard) (op)<br />[cr:hasMaterial](https://w3id.org/cr#hasMaterial) (op)<br />[cr:hasDimensionParameter](https://w3id.org/cr#hasDimensionParameter) (op)<br />[cr:hasPerformanceParameter](https://w3id.org/cr#hasPerformanceParameter) (op)<br />[cr:hasUse](https://w3id.org/cr#hasUse) (op)<br />[cr:rent](https://w3id.org/cr#rent) (dp)<br />[cr:yield](https://w3id.org/cr#yield) (dp)<br />[cr:hasOtherStandard](https://w3id.org/cr#hasOtherStandard) (op)<br />[cr:cam](https://w3id.org/cr#cam) (dp)<br />[cr:hasPhysicalParameter](https://w3id.org/cr#hasPhysicalParameter) (op)<br />[cr:minimunLevelLabourResource](https://w3id.org/cr#minimunLevelLabourResource) (dp)<br />[cr:accessory](https://w3id.org/cr#accessory) (dp)<br />[cr:hasFunction](https://w3id.org/cr#hasFunction) (op)<br />
### Family
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Family`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasFamily](https://w3id.org/cr#hasFamily) (op) **exactly** 1 [cr:Family](https://w3id.org/cr#Family) (c)<br />
Sub-classes |[cr:FamilyOfLabour](https://w3id.org/cr#FamilyOfLabour) (c)<br />[cr:FamilyOfMaterial](https://w3id.org/cr#FamilyOfMaterial) (c)<br />[cr:FamilyOfEquipment](https://w3id.org/cr#FamilyOfEquipment) (c)<br />
In range of |[cr:hasFamily](https://w3id.org/cr#hasFamily) (op)<br />
### Family of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#FamilyOfEquipment`
Super-classes |[cr:Family](https://w3id.org/cr#Family) (c)<br />
### Family of labour
Property | Value
--- | ---
IRI | `https://w3id.org/cr#FamilyOfLabour`
Super-classes |[cr:Family](https://w3id.org/cr#Family) (c)<br />
### Family of material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#FamilyOfMaterial`
Super-classes |[cr:Family](https://w3id.org/cr#Family) (c)<br />
### Finishing
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Finishing`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasFinishing](https://w3id.org/cr#hasFinishing) (op) **max** 5 [cr:Finishing](https://w3id.org/cr#Finishing) (c)<br />
In range of |[cr:hasFinishing](https://w3id.org/cr#hasFinishing) (op)<br />
### Function
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Function`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasFunction](https://w3id.org/cr#hasFunction) (op) **max** 5 [cr:Function](https://w3id.org/cr#Function) (c)<br />
Sub-classes |[cr:FunctionOfEquipment](https://w3id.org/cr#FunctionOfEquipment) (c)<br />[cr:FunctionOfMaterial](https://w3id.org/cr#FunctionOfMaterial) (c)<br />
In range of |[cr:hasFunction](https://w3id.org/cr#hasFunction) (op)<br />
### Function of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#FunctionOfEquipment`
Super-classes |[cr:Function](https://w3id.org/cr#Function) (c)<br />
### Function of material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#FunctionOfMaterial`
Super-classes |[cr:Function](https://w3id.org/cr#Function) (c)<br />
### Furnishing
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Furnishing`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasFurnishing](https://w3id.org/cr#hasFurnishing) (op) **max** 5 [cr:Furnishing](https://w3id.org/cr#Furnishing) (c)<br />
In range of |[cr:hasFurnishing](https://w3id.org/cr#hasFurnishing) (op)<br />
### Gender
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Gender`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasGender](https://w3id.org/cr#hasGender) (op) **exactly** 1 [cr:Gender](https://w3id.org/cr#Gender) (c)<br />
### Labour resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#LabourResource`
Super-classes |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Restrictions |[cr:hasFamily](https://w3id.org/cr#hasFamily) (op) **exactly** 1 [cr:FamilyOfLabour](https://w3id.org/cr#FamilyOfLabour) (c)<br />[cr:hasObject](https://w3id.org/cr#hasObject) (op) **exactly** 1 [cr:ObjectOfLabour](https://w3id.org/cr#ObjectOfLabour) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfLabour](https://w3id.org/cterm#CategoryOfLabour) (c)<br />[cr:hasQualificationLevel](https://w3id.org/cr#hasQualificationLevel) (op) **max** 1 [cr:QualificationLevel](https://w3id.org/cr#QualificationLevel) (c)<br />
In domain of |[cr:hasQualificationLevel](https://w3id.org/cr#hasQualificationLevel) (op)<br />
### Material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Material`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasMaterial](https://w3id.org/cr#hasMaterial) (op) **exactly** 1 [cr:Material](https://w3id.org/cr#Material) (c)<br />
In range of |[cr:hasMaterial](https://w3id.org/cr#hasMaterial) (op)<br />
### Material resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#MaterialResource`
Super-classes |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Restrictions |[cr:hasOtherStandard](https://w3id.org/cr#hasOtherStandard) (op) **max** 5 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfMaterial](https://w3id.org/cterm#CategoryOfMaterial) (c)<br />[cr:hasFinishing](https://w3id.org/cr#hasFinishing) (op) **max** 5 [cr:Finishing](https://w3id.org/cr#Finishing) (c)<br />[cr:hasFurnishing](https://w3id.org/cr#hasFurnishing) (op) **max** 5 [cr:Furnishing](https://w3id.org/cr#Furnishing) (c)<br />[cr:hasFamily](https://w3id.org/cr#hasFamily) (op) **exactly** 1 [cr:FamilyOfMaterial](https://w3id.org/cr#FamilyOfMaterial) (c)<br />[cr:hasFunction](https://w3id.org/cr#hasFunction) (op) **max** 5 [cr:FunctionOfMaterial](https://w3id.org/cr#FunctionOfMaterial) (c)<br />[cterm:hasAspect](https://w3id.org/cterm#hasAspect) **max** 5 [cterm:AspectOfMaterial](https://w3id.org/cterm#AspectOfMaterial) (c)<br />[cr:cam](https://w3id.org/cr#cam) (dp) **exactly** 1<br />[cr:hasUse](https://w3id.org/cr#hasUse) (op) **max** 5 [cr:Use](https://w3id.org/cr#Use) (c)<br />[cr:hasObjectStandard](https://w3id.org/cr#hasObjectStandard) (op) **max** 1 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:hasObject](https://w3id.org/cr#hasObject) (op) **exactly** 1 [cr:ObjectOfMaterial](https://w3id.org/cr#ObjectOfMaterial) (c)<br />[cr:hasPhysicalParameter](https://w3id.org/cr#hasPhysicalParameter) (op) **max** 10 [cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />[cr:hasMaterial](https://w3id.org/cr#hasMaterial) (op) **exactly** 1 [cr:Material](https://w3id.org/cr#Material) (c)<br />[cr:hasDimensionParameter](https://w3id.org/cr#hasDimensionParameter) (op) **max** 10 [cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />[cr:hasPerformanceParameter](https://w3id.org/cr#hasPerformanceParameter) (op) **max** 10 [cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />
In domain of |[cr:hasMaterial](https://w3id.org/cr#hasMaterial) (op)<br />[cr:hasUse](https://w3id.org/cr#hasUse) (op)<br />[cr:hasPerformanceParameter](https://w3id.org/cr#hasPerformanceParameter) (op)<br />[cr:hasFinishing](https://w3id.org/cr#hasFinishing) (op)<br />[cr:hasObjectStandard](https://w3id.org/cr#hasObjectStandard) (op)<br />[cr:hasDimensionParameter](https://w3id.org/cr#hasDimensionParameter) (op)<br />[cr:hasOtherStandard](https://w3id.org/cr#hasOtherStandard) (op)<br />[cr:yield](https://w3id.org/cr#yield) (dp)<br />[cr:hasFurnishing](https://w3id.org/cr#hasFurnishing) (op)<br />[cr:cam](https://w3id.org/cr#cam) (dp)<br />[cr:hasPhysicalParameter](https://w3id.org/cr#hasPhysicalParameter) (op)<br />[cr:hasFunction](https://w3id.org/cr#hasFunction) (op)<br />[cr:hasConsumption](https://w3id.org/cr#hasConsumption) (op)<br />
### oObject
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Object`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasObject](https://w3id.org/cr#hasObject) (op) **exactly** 1 [cr:Object](https://w3id.org/cr#Object) (c)<br />
Sub-classes |[cr:ObjectOfMaterial](https://w3id.org/cr#ObjectOfMaterial) (c)<br />[cr:ObjectOfEquipment](https://w3id.org/cr#ObjectOfEquipment) (c)<br />[cr:ObjectOfLabour](https://w3id.org/cr#ObjectOfLabour) (c)<br />
In range of |[cr:hasObject](https://w3id.org/cr#hasObject) (op)<br />
### Object of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ObjectOfEquipment`
Super-classes |[cr:Object](https://w3id.org/cr#Object) (c)<br />
### Object of labour
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ObjectOfLabour`
Super-classes |[cr:Object](https://w3id.org/cr#Object) (c)<br />
### Object of material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ObjectOfMaterial`
Super-classes |[cr:Object](https://w3id.org/cr#Object) (c)<br />
### Parameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Parameter`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp) **max** 1<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp) **max** 1<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op) **max** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp) **max** 1<br />[cr:hasParameterStandard](https://w3id.org/cr#hasParameterStandard) (op) **max** 1 [cr:Standard](https://w3id.org/cr#Standard) (c)<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp) **max** 1<br />[cr:parameterType](https://w3id.org/cr#parameterType) (dp) **max** 1<br />
Sub-classes |[cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />[cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />[cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />
In domain of |[cr:parameterSymbol1](https://w3id.org/cr#parameterSymbol1) (dp)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op)<br />[cr:hasParameterStandard](https://w3id.org/cr#hasParameterStandard) (op)<br />[cr:parameterValue1](https://w3id.org/cr#parameterValue1) (dp)<br />[cr:parameterValue2](https://w3id.org/cr#parameterValue2) (dp)<br />[cr:parameterSymbol2](https://w3id.org/cr#parameterSymbol2) (dp)<br />[cr:parameterType](https://w3id.org/cr#parameterType) (dp)<br />
### PerformanceParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#PerformanceParameter`
Super-classes |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
In range of |[cr:hasPerformanceParameter](https://w3id.org/cr#hasPerformanceParameter) (op)<br />
### PhysicalParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#PhysicalParameter`
Super-classes |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
In range of |[cr:hasPhysicalParameter](https://w3id.org/cr#hasPhysicalParameter) (op)<br />
### QualificationLevel
Property | Value
--- | ---
IRI | `https://w3id.org/cr#QualificationLevel`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasQualificationLevel](https://w3id.org/cr#hasQualificationLevel) (op) **max** 1 [cr:QualificationLevel](https://w3id.org/cr#QualificationLevel) (c)<br />
In range of |[cr:hasQualificationLevel](https://w3id.org/cr#hasQualificationLevel) (op)<br />
### Resource
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Resource`
Description | <p>This class is used for providing information about a construction resource.</p>
Restrictions |[cr:hasUnit](https://w3id.org/cr#hasUnit) (op) **exactly** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />[cr:descriptionDetail](https://w3id.org/cr#descriptionDetail) (dp) **max** 1<br />[cr:quantityUnitOfMeasure](https://w3id.org/cr#quantityUnitOfMeasure) (dp) **exactly** 1<br />[cr:keywords](https://w3id.org/cr#keywords) (dp) **max** 10<br />[cr:hasType](https://w3id.org/cr#hasType) (op) **max** 1 [cr:Type](https://w3id.org/cr#Type) (c)<br />[cr:law](https://w3id.org/cr#law) (dp) **max** 10<br />[cr:hasGender](https://w3id.org/cr#hasGender) (op) **exactly** 1 [cr:Gender](https://w3id.org/cr#Gender) (c)<br />[cr:descriptionGeneral](https://w3id.org/cr#descriptionGeneral) (dp) **exactly** 1<br />[cr:code](https://w3id.org/cr#code) (dp) **exactly** 1<br />
Sub-classes |[cr:LabourResource](https://w3id.org/cr#LabourResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
In domain of |[cr:law](https://w3id.org/cr#law) (dp)<br />[cr:hasUnit](https://w3id.org/cr#hasUnit) (op)<br />[cr:techSpecs](https://w3id.org/cr#techSpecs) (dp)<br />[cr:hasObject](https://w3id.org/cr#hasObject) (op)<br />[cr:subRecourceOf](https://w3id.org/cr#subRecourceOf)<br />[cr:quantityUnitOfMeasure](https://w3id.org/cr#quantityUnitOfMeasure) (dp)<br />[cr:descriptionGeneral](https://w3id.org/cr#descriptionGeneral) (dp)<br />[cr:hasSubResource](https://w3id.org/cr#hasSubResource)<br />[cr:included](https://w3id.org/cr#included) (dp)<br />[cr:omniclass](https://w3id.org/cr#omniclass) (dp)<br />[cr:hasFamily](https://w3id.org/cr#hasFamily) (op)<br />[cr:uniformat](https://w3id.org/cr#uniformat) (dp)<br />[cr:hasType](https://w3id.org/cr#hasType) (op)<br />[cr:keywords](https://w3id.org/cr#keywords) (dp)<br />[cr:code](https://w3id.org/cr#code) (dp)<br />[cr:escluded](https://w3id.org/cr#escluded) (dp)<br />[cr:hasGender](https://w3id.org/cr#hasGender) (op)<br />[cr:descriptionDetail](https://w3id.org/cr#descriptionDetail) (dp)<br />[cr:uniclass](https://w3id.org/cr#uniclass) (dp)<br />[cr:measurementRules](https://w3id.org/cr#measurementRules) (dp)<br />
In range of |[cr:hasSubResource](https://w3id.org/cr#hasSubResource)<br />[cr:subRecourceOf](https://w3id.org/cr#subRecourceOf)<br />[cr:refResource](https://w3id.org/cr#refResource) (op)<br />
### Resource to cost item assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ResourceToCostItemAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refResource](https://w3id.org/cr#refResource) (op) **some** [cr:Resource](https://w3id.org/cr#Resource) (c)<br />[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [ci:ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />
### Resource to task assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#ResourceToTaskAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refTask](https://w3id.org/cr#refTask) (op) **some** [dtc:Task](https://dtc-ontology.cms.ed.tum.de/ontology/Task) (c)<br />[cr:refResource](https://w3id.org/cr#refResource) (op) **some** [cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Sub-classes |[https://dtc-ontology.cms.ed.tum.de/ontology#ResourceApplication](https://dtc-ontology.cms.ed.tum.de/ontology#ResourceApplication) (c)<br />
### Standard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Standard`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:standardNumber](https://w3id.org/cr#standardNumber) (dp) **max** 1<br />[cr:standardYear](https://w3id.org/cr#standardYear) (dp) **max** 1<br />[cr:standardBody](https://w3id.org/cr#standardBody) (dp) **max** 1<br />[cr:standardPart](https://w3id.org/cr#standardPart) (dp) **max** 1<br />
In domain of |[cr:standardYear](https://w3id.org/cr#standardYear) (dp)<br />[cr:standardBody](https://w3id.org/cr#standardBody) (dp)<br />[cr:standardNumber](https://w3id.org/cr#standardNumber) (dp)<br />[cr:standardPart](https://w3id.org/cr#standardPart) (dp)<br />
In range of |[cr:hasOtherStandard](https://w3id.org/cr#hasOtherStandard) (op)<br />[cr:hasObjectStandard](https://w3id.org/cr#hasObjectStandard) (op)<br />[cr:hasParameterStandard](https://w3id.org/cr#hasParameterStandard) (op)<br />
### Task to geometry assignment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#TaskToGeometryAssignment`
Super-classes |[cr:Assignment](https://w3id.org/cr#Assignment) (c)<br />
Restrictions |[cr:refTask](https://w3id.org/cr#refTask) (op) **some** [dtc:Task](https://dtc-ontology.cms.ed.tum.de/ontology/Task) (c)<br />[cr:refCostItem](https://w3id.org/cr#refCostItem) (op) **some** [http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct](http://ifcowl.openbimstandards.org/IFC4_ADD2#IfcProduct) (c)<br />
### Type
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Type`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cr:hasType](https://w3id.org/cr#hasType) (op) **max** 1 [cr:Type](https://w3id.org/cr#Type) (c)<br />
Sub-classes |[cr:TypeOfLabour](https://w3id.org/cr#TypeOfLabour) (c)<br />[cr:TypeOfMaterial](https://w3id.org/cr#TypeOfMaterial) (c)<br />[cr:TypeOfEquipment](https://w3id.org/cr#TypeOfEquipment) (c)<br />
In range of |[cr:hasType](https://w3id.org/cr#hasType) (op)<br />
### Type of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#TypeOfEquipment`
Super-classes |[cr:Type](https://w3id.org/cr#Type) (c)<br />
### Type of labour
Property | Value
--- | ---
IRI | `https://w3id.org/cr#TypeOfLabour`
Super-classes |[cr:Type](https://w3id.org/cr#Type) (c)<br />
### Type of material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#TypeOfMaterial`
Super-classes |[cr:Type](https://w3id.org/cr#Type) (c)<br />
### Use
Property | Value
--- | ---
IRI | `https://w3id.org/cr#Use`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[cr:UseOfEquipment](https://w3id.org/cr#UseOfEquipment) (c)<br />[cr:UseOfMaterial](https://w3id.org/cr#UseOfMaterial) (c)<br />
In range of |[cr:hasUse](https://w3id.org/cr#hasUse) (op)<br />
### Use of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cr#UseOfEquipment`
Super-classes |[cr:Use](https://w3id.org/cr#Use) (c)<br />
### Use of material
Property | Value
--- | ---
IRI | `https://w3id.org/cr#UseOfMaterial`
Super-classes |[cr:Use](https://w3id.org/cr#Use) (c)<br />

## Object Properties
[hasConsumption](#hasConsumption),
[hasDimensionParameter](#hasDimensionParameter),
[hasFamily](#hasFamily),
[hasFinishing](#hasFinishing),
[hasFunction](#hasFunction),
[hasFurnishing](#hasFurnishing),
[hasGender](#hasGender),
[hasMaterial](#hasMaterial),
[hasObject](#hasObject),
[hasObjectStandard](#hasObjectStandard),
[hasOtherStandard](#hasOtherStandard),
[hasParameterStandard](#hasParameterStandard),
[hasPerformanceParameter](#hasPerformanceParameter),
[resourcePhysicalParameter](#resourcePhysicalParameter),
[hasQualificationLevel](#hasQualificationLevel),
[hasType](#hasType),
[hasUnit](#hasUnit),
[hasUse](#hasUse),
[ref](#ref),
[ref cost item](#refcostitem),
[ref geometry](#refgeometry),
[ref resource](#refresource),
[ref task](#reftask),
[](hasConsumption)
### hasConsumption
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasConsumption`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
[](hasDimensionParameter)
### hasDimensionParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasDimensionParameter`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:DimensionParameter](https://w3id.org/cr#DimensionParameter) (c)<br />
[](hasFamily)
### hasFamily
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasFamily`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[cr:Family](https://w3id.org/cr#Family) (c)<br />
[](hasFinishing)
### hasFinishing
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasFinishing`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:Finishing](https://w3id.org/cr#Finishing) (c)<br />
[](hasFunction)
### hasFunction
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasFunction`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:Function](https://w3id.org/cr#Function) (c)<br />
[](hasFurnishing)
### hasFurnishing
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasFurnishing`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:Furnishing](https://w3id.org/cr#Furnishing) (c)<br />
[](hasGender)
### hasGender
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasGender`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[ci:Gender](https://w3id.org/ci#Gender) (c)<br />
[](hasMaterial)
### hasMaterial
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasMaterial`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:Material](https://w3id.org/cr#Material) (c)<br />
[](hasObject)
### hasObject
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasObject`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[cr:Object](https://w3id.org/cr#Object) (c)<br />
[](hasObjectStandard)
### hasObjectStandard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasObjectStandard`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
[](hasOtherStandard)
### hasOtherStandard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasOtherStandard`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
[](hasParameterStandard)
### hasParameterStandard
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasParameterStandard`
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[cr:Standard](https://w3id.org/cr#Standard) (c)<br />
[](hasPerformanceParameter)
### hasPerformanceParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasPerformanceParameter`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:PerformanceParameter](https://w3id.org/cr#PerformanceParameter) (c)<br />
[](resourcePhysicalParameter)
### resourcePhysicalParameter
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasPhysicalParameter`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />
Range(s) |[cr:PhysicalParameter](https://w3id.org/cr#PhysicalParameter) (c)<br />
[](hasQualificationLevel)
### hasQualificationLevel
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasQualificationLevel`
Domain(s) |[cr:LabourResource](https://w3id.org/cr#LabourResource) (c)<br />
Range(s) |[cr:QualificationLevel](https://w3id.org/cr#QualificationLevel) (c)<br />
[](hasType)
### hasType
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasType`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[cr:Type](https://w3id.org/cr#Type) (c)<br />
[](hasUnit)
### hasUnit
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasUnit`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
Range(s) |[qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />
[](hasUse)
### hasUse
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasUse`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cr:Use](https://w3id.org/cr#Use) (c)<br />
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
Range(s) |[ci:ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />
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

## Datatype Properties
[accessory](#accessory),
[cam](#cam),
[code](#code),
[descriptionDetail](#descriptionDetail),
[descriptionGeneral](#descriptionGeneral),
[escluded](#escluded),
[included](#included),
[keywords](#keywords),
[law](#law),
[measurement rules](#measurementrules),
[minimunLevelLabourResource](#minimunLevelLabourResource),
[omniclass](#omniclass),
[parameterSymbol1](#parameterSymbol1),
[parameterSymbol2](#parameterSymbol2),
[parameterType](#parameterType),
[parameterValue1](#parameterValue1),
[parameterValue2](#parameterValue2),
[quantityUnitOfMeasure](#quantityUnitOfMeasure),
[rent](#rent),
[standardBody](#standardBody),
[standardNumber](#standardNumber),
[standardPart](#standardPart),
[standardYear](#standardYear),
[tech specs](#techspecs),
[uniclass](#uniclass),
[uniformat](#uniformat),
[yield](#yield),
[](accessory)
### accessory
Property | Value
--- | ---
IRI | `https://w3id.org/cr#accessory`
Domain(s) |[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />
[](cam)
### cam
Property | Value
--- | ---
IRI | `https://w3id.org/cr#cam`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />
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
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterSymbol2)
### parameterSymbol2
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterSymbol2`
Domain(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterType)
### parameterType
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterType`
Domain(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterValue1)
### parameterValue1
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterValue1`
Domain(s) |[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](parameterValue2)
### parameterValue2
Property | Value
--- | ---
IRI | `https://w3id.org/cr#parameterValue2`
Domain(s) |[cr:Parameter](https://w3id.org/cr#Parameter) (c)<br />[cr:Consumption](https://w3id.org/cr#Consumption) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
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
[](yield)
### yield
Property | Value
--- | ---
IRI | `https://w3id.org/cr#yield`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />

## Named Individuals
## Namespaces
* **ci**
  * `https://w3id.org/ci#`
* **cr**
  * `https://w3id.org/cr#`
* **cterm**
  * `https://w3id.org/cterm#`
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