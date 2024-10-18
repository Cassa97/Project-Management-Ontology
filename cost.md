Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# The Construction Resources (CR) Ontology

## Metadata
* **IRI**
  * `http://w3id.org/ci`
* **Creators(s)**
  * [Jacopo Cassandro](https://orcid.org/0000-0001-6058-7614)
    [[ORCID]](https://orcid.org/0000-0001-6058-7614)
    (<jacopo.cassandro@polimi.it></a>) of [Politecnico di Milano](https://www.inf.bi.ruhr-uni-bochum.de/iib/lehrstuhl/mitarbeiter/sven_zentgraf.html.en)
* **Contributor(s)**
  * [Claudio Mirarchi](https://orcid.org/0000-0002-6249-243X)
    [[ORCID]](https://orcid.org/0000-0002-6249-243X)
    (<philipp.hagedorn-n6v@rub.de></a>) of [Politecnico di Milano](https://www.inf.bi.ruhr-uni-bochum.de/iib/lehrstuhl/mitarbeiter/philipp_hagedorn.html.en)
  * [Philipp Hagedorn](https://orcid.org/0000-0002-6249-243X)
    [[ORCID]](https://orcid.org/0000-0002-6249-243X)
    (<philipp.hagedorn-n6v@rub.de></a>) of [Ruhr University Bochum](https://www.inf.bi.ruhr-uni-bochum.de/iib/lehrstuhl/mitarbeiter/philipp_hagedorn.html.en)
* **Created**
  * 2024-12-12
* **Version Information**
  * Created with TopBraid Composer
* **Imports**
  * [http://w3id.org/cr](http://w3id.org/cr)
  * [http://w3id.org/cterm](http://w3id.org/cterm)
* **License &amp; Rights**
  * [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
  * &copy; 2024 by DABC, PoliMi
* **Source**
  * [https://linkedbuildingdata.net/ldac2024/files/papers/LDAC2024_Camera_8.pdf](https://linkedbuildingdata.net/ldac2024/files/papers/LDAC2024_Camera_8.pdf)
* **Ontology RDF**
  * RDF ([cost.ttl](turtle))
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
[Activity](#Activity),
[ConstructionWork](#ConstructionWork),
[CostComponent](#CostComponent),
[CostItem](#CostItem),
[DimensionParameter](#DimensionParameter),
[Family](#Family),
[FamilyOfActivity](#FamilyOfActivity),
[FamilyOfCostComponent](#FamilyOfCostComponent),
[FamilyOfWork](#FamilyOfWork),
[Finishing](#Finishing),
[FinishingOfWorkOfConstructionWork](#FinishingOfWorkOfConstructionWork),
[FinishingOfWorkOfProductWork](#FinishingOfWorkOfProductWork),
[FinishingOfWorkOfTemporaryWork](#FinishingOfWorkOfTemporaryWork),
[Function](#Function),
[FunctionOfActivity](#FunctionOfActivity),
[FunctionOfWorkOfConstructionWork](#FunctionOfWorkOfConstructionWork),
[FunctionOfWorkOfProductWork](#FunctionOfWorkOfProductWork),
[FunctionOfWorkOfTemporaryWork](#FunctionOfWorkOfTemporaryWork),
[Gender](#Gender),
[Material](#Material),
[Object](#Object),
[ObjectOfActivity](#ObjectOfActivity),
[ObjectOfCostComponent](#ObjectOfCostComponent),
[ObjectOfWorkOfConstructionWork](#ObjectOfWorkOfConstructionWork),
[ObjectOfWorkOfProductWork](#ObjectOfWorkOfProductWork),
[ObjectOfWorkOfTemporaryWork](#ObjectOfWorkOfTemporaryWork),
[Parameter](#Parameter),
[PerformanceParameter](#PerformanceParameter),
[PhysicalParameter](#PhysicalParameter),
[ProductWork](#ProductWork),
[ProductionResult](#ProductionResult),
[Standard](#Standard),
[TemporaryWork](#TemporaryWork),
[Type](#Type),
[Type of construction work](#Typeofconstructionwork),
[TypeOfActivity](#TypeOfActivity),
[TypeOfProductWork](#TypeOfProductWork),
[TypeOfTemporaryWork](#TypeOfTemporaryWork),
[TypeOfWorkOfConstructionWork](#TypeOfWorkOfConstructionWork),
[TypeOfWorkOfProductWork](#TypeOfWorkOfProductWork),
[TypeOfWorkOfTemporaryWork](#TypeOfWorkOfTemporaryWork),
[Use](#Use),
[UseOfActivity](#UseOfActivity),
[UseOfWorkOfConstructionWork](#UseOfWorkOfConstructionWork),
[UseOfWorkOfProductWork](#UseOfWorkOfProductWork),
[UseOfWorkOfTemporaryWork](#UseOfWorkOfTemporaryWork),
[Work](#Work),
[WorkOfConstructionWork](#WorkOfConstructionWork),
[WorkOfProductWork](#WorkOfProductWork),
[WorkOfTemporaryWork](#WorkOfTemporaryWork),
### Activity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Activity`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:descriptionGeneral](https://w3id.org/ci#descriptionGeneral) (dp) **exactly** 1<br />[ci:descriptionDetail](https://w3id.org/ci#descriptionDetail) (dp) **max** 1<br />[ci:hasFunction](https://w3id.org/ci#hasFunction) (op) **max** 5 [ci:FunctionOfActivity](https://w3id.org/ci#FunctionOfActivity) (c)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op) **exactly** 1 [ci:ObjectOfActivity](https://w3id.org/ci#ObjectOfActivity) (c)<br />[ci:hasFamily](https://w3id.org/ci#hasFamily) (op) **exactly** 1 [ci:FamilyOfActivity](https://w3id.org/ci#FamilyOfActivity) (c)<br />[ci:quantityUnitOfMeasure](https://w3id.org/ci#quantityUnitOfMeasure) (dp) **exactly** 1<br />[ci:hasUse](https://w3id.org/ci#hasUse) (op) **max** 5 [ci:UseOfActivity](https://w3id.org/ci#UseOfActivity) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfActivity](https://w3id.org/cterm#CategoryOfActivity) (c)<br />[ci:hasType](https://w3id.org/ci#hasType) (op) **max** 1 [ci:TypeOfActivity](https://w3id.org/ci#TypeOfActivity) (c)<br />[ci:unitPrice](https://w3id.org/ci#unitPrice) (dp) **exactly** 1<br />[ci:hasGender](https://w3id.org/ci#hasGender) (op) **exactly** 1 [ci:Gender](https://w3id.org/ci#Gender) (c)<br />[ci:hasSubComponent](https://w3id.org/ci#hasSubComponent) (op) **some** [ci:TemporaryWork](https://w3id.org/ci#TemporaryWork) (c)<br />[ci:code](https://w3id.org/ci#code) (dp) **exactly** 1<br />
In domain of |[ci:hasType](https://w3id.org/ci#hasType) (op)<br />[ci:keywords](https://w3id.org/ci#keywords) (dp)<br />[ci:hasSubComponent](https://w3id.org/ci#hasSubComponent) (op)<br />[ci:hasFamily](https://w3id.org/ci#hasFamily) (op)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op)<br />[ci:hasGender](https://w3id.org/ci#hasGender) (op)<br />[ci:hasUse](https://w3id.org/ci#hasUse) (op)<br />[ci:hasUnit](https://w3id.org/ci#hasUnit) (op)<br />[ci:hasFunction](https://w3id.org/ci#hasFunction) (op)<br />[ci:hasOtherStandard](https://w3id.org/ci#hasOtherStandard) (op)<br />[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op)<br />
In range of |[ci:hasActivity](https://w3id.org/ci#hasActivity) (op)<br />
### ConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ConstructionWork`
Super-classes |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Restrictions |[ci:hasType](https://w3id.org/ci#hasType) (op) **max** 1 [ci:TypeOfConstructionWork](https://w3id.org/ci#TypeOfConstructionWork) (c)<br />[ci:hasWork](https://w3id.org/ci#hasWork) (op) **exactly** 1 [ci:WorkOfConstructionWork](https://w3id.org/ci#WorkOfConstructionWork) (c)<br />[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op) **max** 1 [ci:Standard](https://w3id.org/ci#Standard) (c)<br />
### CostComponent
Property | Value
--- | ---
IRI | `https://w3id.org/ci#CostComponent`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasGender](https://w3id.org/ci#hasGender) (op) **exactly** 1 [ci:Gender](https://w3id.org/ci#Gender) (c)<br />[ci:descriptionDetail](https://w3id.org/ci#descriptionDetail) (dp) **max** 1<br />[ci:quantityUnitOfMeasure](https://w3id.org/ci#quantityUnitOfMeasure) (dp) **exactly** 1<br />[ci:unitPrice](https://w3id.org/ci#unitPrice) (dp) **exactly** 1<br />[ci:hasFamily](https://w3id.org/ci#hasFamily) (op) **exactly** 1 [ci:FamilyOfCostComponent](https://w3id.org/ci#FamilyOfCostComponent) (c)<br />[ci:IsPartOf](https://w3id.org/ci#IsPartOf) (op) **some** [ci:CostItem](https://w3id.org/ci#CostItem) (c)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op) **exactly** 1 [ci:ObjectOfCostComponent](https://w3id.org/ci#ObjectOfCostComponent) (c)<br />[ci:code](https://w3id.org/ci#code) (dp) **exactly** 1<br />[ci:hasActivity](https://w3id.org/ci#hasActivity) (op) **exactly** 1 [ci:Activity](https://w3id.org/ci#Activity) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfCostComponent](https://w3id.org/cterm#CategoryOfCostComponent) (c)<br />[ci:hasMaterial](https://w3id.org/ci#hasMaterial) (op) **exactly** 1 [ci:Material](https://w3id.org/ci#Material) (c)<br />[ci:descriptionGeneral](https://w3id.org/ci#descriptionGeneral) (dp) **exactly** 1<br />
Sub-classes |[ci:ConstructionWork](https://w3id.org/ci#ConstructionWork) (c)<br />[ci:ProductWork](https://w3id.org/ci#ProductWork) (c)<br />[ci:TemporaryWork](https://w3id.org/ci#TemporaryWork) (c)<br />
In domain of |[ci:measurementRules](https://w3id.org/ci#measurementRules) (dp)<br />[ci:hasGender](https://w3id.org/ci#hasGender) (op)<br />[ci:uniclass](https://w3id.org/ci#uniclass) (dp)<br />[ci:omniclass](https://w3id.org/ci#omniclass) (dp)<br />[ci:code](https://w3id.org/ci#code) (dp)<br />[ci:hasUnit](https://w3id.org/ci#hasUnit) (op)<br />[ci:escluded](https://w3id.org/ci#escluded) (dp)<br />[ci:unitPrice](https://w3id.org/ci#unitPrice) (dp)<br />[ci:hasWork](https://w3id.org/ci#hasWork) (op)<br />[ci:IsPartOf](https://w3id.org/ci#IsPartOf) (op)<br />[ci:hasType](https://w3id.org/ci#hasType) (op)<br />[ci:hasMaterial](https://w3id.org/ci#hasMaterial) (op)<br />[ci:techSpecs](https://w3id.org/ci#techSpecs) (dp)<br />[ci:hasFamily](https://w3id.org/ci#hasFamily) (op)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op)<br />[ci:hasActivity](https://w3id.org/ci#hasActivity) (op)<br />[ci:included](https://w3id.org/ci#included) (dp)<br />[ci:uniformat](https://w3id.org/ci#uniformat) (dp)<br />[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op)<br />[ci:hasOtherStandard](https://w3id.org/ci#hasOtherStandard) (op)<br />[ci:descriptionGeneral](https://w3id.org/ci#descriptionGeneral) (dp)<br />[ci:quantityUnitOfMeasure](https://w3id.org/ci#quantityUnitOfMeasure) (dp)<br />[ci:descriptionDetail](https://w3id.org/ci#descriptionDetail) (dp)<br />
In range of |[ci:hasSubComponent](https://w3id.org/ci#hasSubComponent) (op)<br />[ci:hasPart](https://w3id.org/ci#hasPart) (op)<br />
### CostItem
Property | Value
--- | ---
IRI | `https://w3id.org/ci#CostItem`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasPart](https://w3id.org/ci#hasPart) (op) **some** [ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
In domain of |[ci:hasPart](https://w3id.org/ci#hasPart) (op)<br />
In range of |[ci:IsPartOf](https://w3id.org/ci#IsPartOf) (op)<br />
### DimensionParameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#DimensionParameter`
Super-classes |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
In range of |[ci:hasDimensionParameter](https://w3id.org/ci#hasDimensionParameter) (op)<br />
### Family
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Family`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasFamily](https://w3id.org/ci#hasFamily) (op) **exactly** 1 [ci:Family](https://w3id.org/ci#Family) (c)<br />
Sub-classes |[ci:FamilyOfCostComponent](https://w3id.org/ci#FamilyOfCostComponent) (c)<br />[ci:FamilyOfWork](https://w3id.org/ci#FamilyOfWork) (c)<br />[ci:FamilyOfActivity](https://w3id.org/ci#FamilyOfActivity) (c)<br />
In range of |[ci:hasFamily](https://w3id.org/ci#hasFamily) (op)<br />
### FamilyOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FamilyOfActivity`
Super-classes |[ci:Family](https://w3id.org/ci#Family) (c)<br />
### FamilyOfCostComponent
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FamilyOfCostComponent`
Super-classes |[ci:Family](https://w3id.org/ci#Family) (c)<br />
### FamilyOfWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FamilyOfWork`
Super-classes |[ci:Family](https://w3id.org/ci#Family) (c)<br />
### Finishing
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Finishing`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasFinishing](https://w3id.org/ci#hasFinishing) (op) **max** 5 [ci:Finishing](https://w3id.org/ci#Finishing) (c)<br />
Sub-classes |[ci:FinishingOfWorkOfTemporaryWork](https://w3id.org/ci#FinishingOfWorkOfTemporaryWork) (c)<br />[ci:FinishingOfWorkOfProductWork](https://w3id.org/ci#FinishingOfWorkOfProductWork) (c)<br />[ci:FinishingOfWorkOfConstructionWork](https://w3id.org/ci#FinishingOfWorkOfConstructionWork) (c)<br />
In range of |[ci:hasFinishing](https://w3id.org/ci#hasFinishing) (op)<br />
### FinishingOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FinishingOfWorkOfConstructionWork`
Super-classes |[ci:Finishing](https://w3id.org/ci#Finishing) (c)<br />
### FinishingOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FinishingOfWorkOfProductWork`
Super-classes |[ci:Finishing](https://w3id.org/ci#Finishing) (c)<br />
### FinishingOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FinishingOfWorkOfTemporaryWork`
Super-classes |[ci:Finishing](https://w3id.org/ci#Finishing) (c)<br />
### Function
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Function`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasFunction](https://w3id.org/ci#hasFunction) (op) **max** 5 [ci:Function](https://w3id.org/ci#Function) (c)<br />
Sub-classes |[ci:FunctionOfWorkOfProductWork](https://w3id.org/ci#FunctionOfWorkOfProductWork) (c)<br />[ci:FunctionOfWorkOfTemporaryWork](https://w3id.org/ci#FunctionOfWorkOfTemporaryWork) (c)<br />[ci:FunctionOfActivity](https://w3id.org/ci#FunctionOfActivity) (c)<br />[ci:FunctionOfWorkOfConstructionWork](https://w3id.org/ci#FunctionOfWorkOfConstructionWork) (c)<br />
In range of |[ci:hasFunction](https://w3id.org/ci#hasFunction) (op)<br />
### FunctionOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FunctionOfActivity`
Super-classes |[ci:Function](https://w3id.org/ci#Function) (c)<br />
### FunctionOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FunctionOfWorkOfConstructionWork`
Super-classes |[ci:Function](https://w3id.org/ci#Function) (c)<br />
### FunctionOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FunctionOfWorkOfProductWork`
Super-classes |[ci:Function](https://w3id.org/ci#Function) (c)<br />
### FunctionOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#FunctionOfWorkOfTemporaryWork`
Super-classes |[ci:Function](https://w3id.org/ci#Function) (c)<br />
### Gender
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Gender`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasGender](https://w3id.org/ci#hasGender) (op) **exactly** 1 [ci:Gender](https://w3id.org/ci#Gender) (c)<br />
In range of |[ci:hasGender](https://w3id.org/ci#hasGender) (op)<br />
### Material
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Material`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasMaterial](https://w3id.org/ci#hasMaterial) (op) **exactly** 1 [ci:Material](https://w3id.org/ci#Material) (c)<br />
In range of |[ci:hasMaterial](https://w3id.org/ci#hasMaterial) (op)<br />
### Object
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Object`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasObject](https://w3id.org/ci#hasObject) (op) **exactly** 1 [ci:Object](https://w3id.org/ci#Object) (c)<br />
Sub-classes |[ci:ObjectOfWorkOfProductWork](https://w3id.org/ci#ObjectOfWorkOfProductWork) (c)<br />[ci:ObjectOfWorkOfTemporaryWork](https://w3id.org/ci#ObjectOfWorkOfTemporaryWork) (c)<br />[ci:ObjectOfActivity](https://w3id.org/ci#ObjectOfActivity) (c)<br />[ci:ObjectOfWorkOfConstructionWork](https://w3id.org/ci#ObjectOfWorkOfConstructionWork) (c)<br />[ci:ObjectOfCostComponent](https://w3id.org/ci#ObjectOfCostComponent) (c)<br />
In range of |[ci:hasObject](https://w3id.org/ci#hasObject) (op)<br />
### ObjectOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ObjectOfActivity`
Super-classes |[ci:Object](https://w3id.org/ci#Object) (c)<br />
### ObjectOfCostComponent
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ObjectOfCostComponent`
Super-classes |[ci:Object](https://w3id.org/ci#Object) (c)<br />
### ObjectOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ObjectOfWorkOfConstructionWork`
Super-classes |[ci:Object](https://w3id.org/ci#Object) (c)<br />
### ObjectOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ObjectOfWorkOfProductWork`
Super-classes |[ci:Object](https://w3id.org/ci#Object) (c)<br />
### ObjectOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ObjectOfWorkOfTemporaryWork`
Super-classes |[ci:Object](https://w3id.org/ci#Object) (c)<br />
### Parameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Parameter`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:parameterValue2](https://w3id.org/ci#parameterValue2) (dp) **max** 1<br />[ci:hasParameterStandard](https://w3id.org/ci#hasParameterStandard) (op) **max** 1 [ci:Standard](https://w3id.org/ci#Standard) (c)<br />[ci:parameterSimbol1](https://w3id.org/ci#parameterSimbol1) (dp) **max** 1<br />[ci:parameterValue1](https://w3id.org/ci#parameterValue1) (dp) **max** 1<br />[ci:parameterSimbol2](https://w3id.org/ci#parameterSimbol2) (dp) **max** 1<br />[ci:parameterType](https://w3id.org/ci#parameterType) (dp) **max** 1<br />[ci:hasUnit](https://w3id.org/ci#hasUnit) (op) **max** 1 [qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />
Sub-classes |[ci:DimensionParameter](https://w3id.org/ci#DimensionParameter) (c)<br />[ci:PerformanceParameter](https://w3id.org/ci#PerformanceParameter) (c)<br />[ci:PhysicalParameter](https://w3id.org/ci#PhysicalParameter) (c)<br />
In domain of |[ci:parameterSimbol2](https://w3id.org/ci#parameterSimbol2) (dp)<br />[ci:parameterSimbol1](https://w3id.org/ci#parameterSimbol1) (dp)<br />[ci:parameterValue2](https://w3id.org/ci#parameterValue2) (dp)<br />[ci:hasParameterStandard](https://w3id.org/ci#hasParameterStandard) (op)<br />[ci:parameterValue1](https://w3id.org/ci#parameterValue1) (dp)<br />[ci:hasUnit](https://w3id.org/ci#hasUnit) (op)<br />[ci:parameterType](https://w3id.org/ci#parameterType) (dp)<br />
### PerformanceParameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#PerformanceParameter`
Super-classes |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
In range of |[ci:hasPerformanceParameter](https://w3id.org/ci#hasPerformanceParameter) (op)<br />
### PhysicalParameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#PhysicalParameter`
Super-classes |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
In range of |[ci:hasPhysicalParameter](https://w3id.org/ci#hasPhysicalParameter) (op)<br />
### ProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ProductWork`
Super-classes |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Restrictions |[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op) **max** 1 [ci:Standard](https://w3id.org/ci#Standard) (c)<br />[ci:hasType](https://w3id.org/ci#hasType) (op) **max** 1 [ci:TypeOfProductWork](https://w3id.org/ci#TypeOfProductWork) (c)<br />[ci:hasWork](https://w3id.org/ci#hasWork) (op) **exactly** 1 [ci:WorkOfProductWork](https://w3id.org/ci#WorkOfProductWork) (c)<br />
### ProductionResult
Property | Value
--- | ---
IRI | `https://w3id.org/ci#ProductionResult`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasPart](https://w3id.org/ci#hasPart) (op) **some** [ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
In domain of |[ci:hasPart](https://w3id.org/ci#hasPart) (op)<br />
In range of |[ci:IsPartOf](https://w3id.org/ci#IsPartOf) (op)<br />
### Standard
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Standard`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:standardPart](https://w3id.org/ci#standardPart) (dp) **max** 1<br />[ci:standardNumber](https://w3id.org/ci#standardNumber) (dp) **max** 1<br />[ci:standardBody](https://w3id.org/ci#standardBody) (dp) **max** 1<br />[ci:standardYear](https://w3id.org/ci#standardYear) (dp) **max** 1<br />
In domain of |[ci:standardNumber](https://w3id.org/ci#standardNumber) (dp)<br />[ci:standardBody](https://w3id.org/ci#standardBody) (dp)<br />[ci:standardPart](https://w3id.org/ci#standardPart) (dp)<br />[ci:standardYear](https://w3id.org/ci#standardYear) (dp)<br />
In range of |[ci:hasParameterStandard](https://w3id.org/ci#hasParameterStandard) (op)<br />[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op)<br />[ci:hasOtherStandard](https://w3id.org/ci#hasOtherStandard) (op)<br />
### TemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TemporaryWork`
Super-classes |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Restrictions |[ci:hasWork](https://w3id.org/ci#hasWork) (op) **exactly** 1 [ci:WorkOfTemporaryWork](https://w3id.org/ci#WorkOfTemporaryWork) (c)<br />[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op) **max** 1 [ci:Standard](https://w3id.org/ci#Standard) (c)<br />[ci:hasType](https://w3id.org/ci#hasType) (op) **max** 1 [ci:TypeOfTemporaryWork](https://w3id.org/ci#TypeOfTemporaryWork) (c)<br />
### Type
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Type`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[ci:TypeOfWorkOfProductWork](https://w3id.org/ci#TypeOfWorkOfProductWork) (c)<br />[ci:TypeOfConstructionWork](https://w3id.org/ci#TypeOfConstructionWork) (c)<br />[ci:TypeOfProductWork](https://w3id.org/ci#TypeOfProductWork) (c)<br />[ci:TypeOfActivity](https://w3id.org/ci#TypeOfActivity) (c)<br />[ci:TypeOfTemporaryWork](https://w3id.org/ci#TypeOfTemporaryWork) (c)<br />[ci:TypeOfWorkOfConstructionWork](https://w3id.org/ci#TypeOfWorkOfConstructionWork) (c)<br />[ci:TypeOfWorkOfTemporaryWork](https://w3id.org/ci#TypeOfWorkOfTemporaryWork) (c)<br />
In range of |[ci:hasType](https://w3id.org/ci#hasType) (op)<br />
### TypeOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfActivity`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### Type of construction work
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfConstructionWork`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### TypeOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfProductWork`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### TypeOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfTemporaryWork`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### TypeOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfWorkOfConstructionWork`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### TypeOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfWorkOfProductWork`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### TypeOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#TypeOfWorkOfTemporaryWork`
Super-classes |[ci:Type](https://w3id.org/ci#Type) (c)<br />
### Use
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Use`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[ci:UseOfWorkOfConstructionWork](https://w3id.org/ci#UseOfWorkOfConstructionWork) (c)<br />[ci:UseOfWorkOfProductWork](https://w3id.org/ci#UseOfWorkOfProductWork) (c)<br />[ci:UseOfWorkOfTemporaryWork](https://w3id.org/ci#UseOfWorkOfTemporaryWork) (c)<br />[ci:UseOfActivity](https://w3id.org/ci#UseOfActivity) (c)<br />
In range of |[ci:hasUse](https://w3id.org/ci#hasUse) (op)<br />
### UseOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#UseOfActivity`
Super-classes |[ci:Use](https://w3id.org/ci#Use) (c)<br />
### UseOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#UseOfWorkOfConstructionWork`
Super-classes |[ci:Use](https://w3id.org/ci#Use) (c)<br />
### UseOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#UseOfWorkOfProductWork`
Super-classes |[ci:Use](https://w3id.org/ci#Use) (c)<br />
### UseOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#UseOfWorkOfTemporaryWork`
Super-classes |[ci:Use](https://w3id.org/ci#Use) (c)<br />
### Work
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Work`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[ci:hasPhysicalParameter](https://w3id.org/ci#hasPhysicalParameter) (op) **max** 10 [ci:PhysicalParameter](https://w3id.org/ci#PhysicalParameter) (c)<br />[ci:quantityUnitOfMeasure](https://w3id.org/ci#quantityUnitOfMeasure) (dp) **exactly** 1<br />[ci:cam](https://w3id.org/ci#cam) (dp) **max** 1<br />[ci:code](https://w3id.org/ci#code) (dp) **exactly** 1<br />[ci:hasGender](https://w3id.org/ci#hasGender) (op) **exactly** 1 [ci:Gender](https://w3id.org/ci#Gender) (c)<br />[ci:hasDimensionParameter](https://w3id.org/ci#hasDimensionParameter) (op) **max** 10 [ci:DimensionParameter](https://w3id.org/ci#DimensionParameter) (c)<br />[ci:unitPrice](https://w3id.org/ci#unitPrice) (dp) **exactly** 1<br />[ci:law](https://w3id.org/ci#law) (dp) **max** 10<br />[ci:hasFamily](https://w3id.org/ci#hasFamily) (op) **exactly** 1 [ci:FamilyOfWork](https://w3id.org/ci#FamilyOfWork) (c)<br />[ci:hasPerformanceParameter](https://w3id.org/ci#hasPerformanceParameter) (op) **max** 10 [ci:PerformanceParameter](https://w3id.org/ci#PerformanceParameter) (c)<br />[ci:descriptionDetail](https://w3id.org/ci#descriptionDetail) (dp) **max** 1<br />[ci:descriptionGeneral](https://w3id.org/ci#descriptionGeneral) (dp) **exactly** 1<br />[ci:hasMaterial](https://w3id.org/ci#hasMaterial) (op) **exactly** 1 [ci:Material](https://w3id.org/ci#Material) (c)<br />[ci:hasOtherStandard](https://w3id.org/ci#hasOtherStandard) (op) **max** 5 [ci:Standard](https://w3id.org/ci#Standard) (c)<br />
Sub-classes |[ci:WorkOfTemporaryWork](https://w3id.org/ci#WorkOfTemporaryWork) (c)<br />[ci:WorkOfConstructionWork](https://w3id.org/ci#WorkOfConstructionWork) (c)<br />[ci:WorkOfProductWork](https://w3id.org/ci#WorkOfProductWork) (c)<br />
In domain of |[ci:hasType](https://w3id.org/ci#hasType) (op)<br />[ci:hasFinishing](https://w3id.org/ci#hasFinishing) (op)<br />[ci:hasMaterial](https://w3id.org/ci#hasMaterial) (op)<br />[ci:hasPerformanceParameter](https://w3id.org/ci#hasPerformanceParameter) (op)<br />[ci:hasFamily](https://w3id.org/ci#hasFamily) (op)<br />[ci:keywords](https://w3id.org/ci#keywords) (dp)<br />[ci:law](https://w3id.org/ci#law) (dp)<br />[ci:cam](https://w3id.org/ci#cam) (dp)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op)<br />[ci:hasUnit](https://w3id.org/ci#hasUnit) (op)<br />[ci:hasFunction](https://w3id.org/ci#hasFunction) (op)<br />[ci:hasUse](https://w3id.org/ci#hasUse) (op)<br />[ci:hasGender](https://w3id.org/ci#hasGender) (op)<br />[ci:hasPhysicalParameter](https://w3id.org/ci#hasPhysicalParameter) (op)<br />[ci:hasObjectStandard](https://w3id.org/ci#hasObjectStandard) (op)<br />[ci:hasOtherStandard](https://w3id.org/ci#hasOtherStandard) (op)<br />[ci:hasDimensionParameter](https://w3id.org/ci#hasDimensionParameter) (op)<br />
In range of |[ci:hasWork](https://w3id.org/ci#hasWork) (op)<br />
### WorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#WorkOfConstructionWork`
Super-classes |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Restrictions |[ci:hasFunction](https://w3id.org/ci#hasFunction) (op) **max** 1 [ci:FunctionOfWorkOfConstructionWork](https://w3id.org/ci#FunctionOfWorkOfConstructionWork) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfWorkOfConstructionWork](https://w3id.org/cterm#CategoryOfWorkOfConstructionWork) (c)<br />[ci:hasFinishing](https://w3id.org/ci#hasFinishing) (op) **max** 5 [ci:FinishingOfWorkOfConstructionWork](https://w3id.org/ci#FinishingOfWorkOfConstructionWork) (c)<br />[ci:hasUse](https://w3id.org/ci#hasUse) (op) **max** 5 [ci:UseOfWorkOfConstructionWork](https://w3id.org/ci#UseOfWorkOfConstructionWork) (c)<br />[ci:hasSubComponent](https://w3id.org/ci#hasSubComponent) (op) **some** [ci:ProductWork](https://w3id.org/ci#ProductWork) (c)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op) **exactly** 1 [ci:ObjectOfWorkOfConstructionWork](https://w3id.org/ci#ObjectOfWorkOfConstructionWork) (c)<br />[ci:hasSubComponent](https://w3id.org/ci#hasSubComponent) (op) **some** [ci:ConstructionWork](https://w3id.org/ci#ConstructionWork) (c)<br />[ci:hasType](https://w3id.org/ci#hasType) (op) **max** 1 [ci:TypeOfWorkOfConstructionWork](https://w3id.org/ci#TypeOfWorkOfConstructionWork) (c)<br />[cterm:hasAspect](https://w3id.org/cterm#hasAspect) **max** 5 [cterm:AspectOfWorkOfConstructionWork](https://w3id.org/cterm#AspectOfWorkOfConstructionWork) (c)<br />
In domain of |[ci:hasSubComponent](https://w3id.org/ci#hasSubComponent) (op)<br />
### WorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#WorkOfProductWork`
Super-classes |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Restrictions |[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfWorkOfProductWork](https://w3id.org/cterm#CategoryOfWorkOfProductWork) (c)<br />[cterm:hasAspect](https://w3id.org/cterm#hasAspect) **max** 5 [cterm:AspectOfWorkOfProductWork](https://w3id.org/cterm#AspectOfWorkOfProductWork) (c)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op) **exactly** 1 [ci:ObjectOfWorkOfProductWork](https://w3id.org/ci#ObjectOfWorkOfProductWork) (c)<br />[ci:hasUse](https://w3id.org/ci#hasUse) (op) **max** 5 [ci:UseOfWorkOfProductWork](https://w3id.org/ci#UseOfWorkOfProductWork) (c)<br />[ci:hasFunction](https://w3id.org/ci#hasFunction) (op) **max** 1 [ci:FunctionOfWorkOfProductWork](https://w3id.org/ci#FunctionOfWorkOfProductWork) (c)<br />[ci:hasType](https://w3id.org/ci#hasType) (op) **max** 1 [ci:TypeOfWorkOfProductWork](https://w3id.org/ci#TypeOfWorkOfProductWork) (c)<br />[ci:hasFinishing](https://w3id.org/ci#hasFinishing) (op) **max** 5 [ci:FinishingOfWorkOfProductWork](https://w3id.org/ci#FinishingOfWorkOfProductWork) (c)<br />
### WorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#WorkOfTemporaryWork`
Super-classes |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Restrictions |[ci:hasUse](https://w3id.org/ci#hasUse) (op) **max** 5 [ci:UseOfWorkOfTemporaryWork](https://w3id.org/ci#UseOfWorkOfTemporaryWork) (c)<br />[ci:hasFinishing](https://w3id.org/ci#hasFinishing) (op) **max** 5 [ci:FinishingOfWorkOfTemporaryWork](https://w3id.org/ci#FinishingOfWorkOfTemporaryWork) (c)<br />[ci:hasFunction](https://w3id.org/ci#hasFunction) (op) **max** 1 [ci:FunctionOfWorkOfTemporaryWork](https://w3id.org/ci#FunctionOfWorkOfTemporaryWork) (c)<br />[ci:hasObject](https://w3id.org/ci#hasObject) (op) **exactly** 1 [ci:ObjectOfWorkOfTemporaryWork](https://w3id.org/ci#ObjectOfWorkOfTemporaryWork) (c)<br />[cterm:hasCategory](https://w3id.org/cterm#hasCategory) **exactly** 1 [cterm:CategoryOfWorkOfTemporaryWork](https://w3id.org/cterm#CategoryOfWorkOfTemporaryWork) (c)<br />[ci:hasType](https://w3id.org/ci#hasType) (op) **exactly** 1 [ci:TypeOfWorkOfTemporaryWork](https://w3id.org/ci#TypeOfWorkOfTemporaryWork) (c)<br />[cterm:hasAspect](https://w3id.org/cterm#hasAspect) **max** 5 [cterm:AspectOfWorkOfTemporaryWork](https://w3id.org/cterm#AspectOfWorkOfTemporaryWork) (c)<br />

## Object Properties
[IsPartOf](#IsPartOf),
[hasActivity](#hasActivity),
[hasDimensionParameter](#hasDimensionParameter),
[hasFamily](#hasFamily),
[hasFinishing](#hasFinishing),
[hasFunction](#hasFunction),
[hasGender](#hasGender),
[hasMaterial](#hasMaterial),
[hasObject](#hasObject),
[hasObjectStandard](#hasObjectStandard),
[hasOtherStandard](#hasOtherStandard),
[hasParameterStandard](#hasParameterStandard),
[hasPart](#hasPart),
[hasPerformanceParameter](#hasPerformanceParameter),
[hasPhysicalParameter](#hasPhysicalParameter),
[hasSubComponent](#hasSubComponent),
[hasType](#hasType),
[hasUnit](#hasUnit),
[hasUse](#hasUse),
[hasWork](#hasWork),
[](IsPartOf)
### IsPartOf
Property | Value
--- | ---
IRI | `https://w3id.org/ci#IsPartOf`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[ci:ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />[ci:CostItem](https://w3id.org/ci#CostItem) (c)<br />
[](hasActivity)
### hasActivity
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasActivity`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[ci:Activity](https://w3id.org/ci#Activity) (c)<br />
[](hasDimensionParameter)
### hasDimensionParameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasDimensionParameter`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:DimensionParameter](https://w3id.org/ci#DimensionParameter) (c)<br />
[](hasFamily)
### hasFamily
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasFamily`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />
Range(s) |[ci:Family](https://w3id.org/ci#Family) (c)<br />
[](hasFinishing)
### hasFinishing
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasFinishing`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:Finishing](https://w3id.org/ci#Finishing) (c)<br />
[](hasFunction)
### hasFunction
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasFunction`
Domain(s) |[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:Function](https://w3id.org/ci#Function) (c)<br />
[](hasGender)
### hasGender
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasGender`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:Gender](https://w3id.org/ci#Gender) (c)<br />
[](hasMaterial)
### hasMaterial
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasMaterial`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[ci:Material](https://w3id.org/ci#Material) (c)<br />
[](hasObject)
### hasObject
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasObject`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:Object](https://w3id.org/ci#Object) (c)<br />
[](hasObjectStandard)
### hasObjectStandard
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasObjectStandard`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />
Range(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
[](hasOtherStandard)
### hasOtherStandard
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasOtherStandard`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
[](hasParameterStandard)
### hasParameterStandard
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasParameterStandard`
Domain(s) |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
Range(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
[](hasPart)
### hasPart
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasPart`
Domain(s) |[ci:CostItem](https://w3id.org/ci#CostItem) (c)<br />[ci:ProductionResult](https://w3id.org/ci#ProductionResult) (c)<br />
Range(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
[](hasPerformanceParameter)
### hasPerformanceParameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasPerformanceParameter`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:PerformanceParameter](https://w3id.org/ci#PerformanceParameter) (c)<br />
[](hasPhysicalParameter)
### hasPhysicalParameter
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasPhysicalParameter`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:PhysicalParameter](https://w3id.org/ci#PhysicalParameter) (c)<br />
[](hasSubComponent)
### hasSubComponent
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasSubComponent`
Domain(s) |[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:WorkOfConstructionWork](https://w3id.org/ci#WorkOfConstructionWork) (c)<br />
Range(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
[](hasType)
### hasType
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasType`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />
Range(s) |[ci:Type](https://w3id.org/ci#Type) (c)<br />
[](hasUnit)
### hasUnit
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasUnit`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />
Range(s) |[qudt:Unit](http://qudt.org/schema/qudt/Unit) (c)<br />
[](hasUse)
### hasUse
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasUse`
Domain(s) |[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[ci:Use](https://w3id.org/ci#Use) (c)<br />
[](hasWork)
### hasWork
Property | Value
--- | ---
IRI | `https://w3id.org/ci#hasWork`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />

## Datatype Properties
[cam](#cam),
[code](#code),
[descriptionDetail](#descriptionDetail),
[descriptionGeneral](#descriptionGeneral),
[escluded](#escluded),
[included](#included),
[keywords](#keywords),
[law](#law),
[measurementRules](#measurementRules),
[omniclass](#omniclass),
[parameterSimbol1](#parameterSimbol1),
[parameterSimbol2](#parameterSimbol2),
[parameterType](#parameterType),
[parameterValue1](#parameterValue1),
[parameterValue2](#parameterValue2),
[quantityUnitOfMeasure](#quantityUnitOfMeasure),
[standardBody](#standardBody),
[standardNumber](#standardNumber),
[standardPart](#standardPart),
[standardYear](#standardYear),
[tech specs](#techspecs),
[uniclass](#uniclass),
[uniformat](#uniformat),
[unit price](#unitprice),
[](cam)
### cam
Property | Value
--- | ---
IRI | `https://w3id.org/ci#cam`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />
[](code)
### code
Property | Value
--- | ---
IRI | `https://w3id.org/ci#code`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](descriptionDetail)
### descriptionDetail
Property | Value
--- | ---
IRI | `https://w3id.org/ci#descriptionDetail`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](descriptionGeneral)
### descriptionGeneral
Property | Value
--- | ---
IRI | `https://w3id.org/ci#descriptionGeneral`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](escluded)
### escluded
Property | Value
--- | ---
IRI | `https://w3id.org/ci#escluded`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](included)
### included
Property | Value
--- | ---
IRI | `https://w3id.org/ci#included`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](keywords)
### keywords
Property | Value
--- | ---
IRI | `https://w3id.org/ci#keywords`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](law)
### law
Property | Value
--- | ---
IRI | `https://w3id.org/ci#law`
Domain(s) |[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](measurementRules)
### measurementRules
Property | Value
--- | ---
IRI | `https://w3id.org/ci#measurementRules`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](omniclass)
### omniclass
Property | Value
--- | ---
IRI | `https://w3id.org/ci#omniclass`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterSimbol1)
### parameterSimbol1
Property | Value
--- | ---
IRI | `https://w3id.org/ci#parameterSimbol1`
Domain(s) |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterSimbol2)
### parameterSimbol2
Property | Value
--- | ---
IRI | `https://w3id.org/ci#parameterSimbol2`
Domain(s) |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterType)
### parameterType
Property | Value
--- | ---
IRI | `https://w3id.org/ci#parameterType`
Domain(s) |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](parameterValue1)
### parameterValue1
Property | Value
--- | ---
IRI | `https://w3id.org/ci#parameterValue1`
Domain(s) |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](parameterValue2)
### parameterValue2
Property | Value
--- | ---
IRI | `https://w3id.org/ci#parameterValue2`
Domain(s) |[ci:Parameter](https://w3id.org/ci#Parameter) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](quantityUnitOfMeasure)
### quantityUnitOfMeasure
Property | Value
--- | ---
IRI | `https://w3id.org/ci#quantityUnitOfMeasure`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](standardBody)
### standardBody
Property | Value
--- | ---
IRI | `https://w3id.org/ci#standardBody`
Domain(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](standardNumber)
### standardNumber
Property | Value
--- | ---
IRI | `https://w3id.org/ci#standardNumber`
Domain(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](standardPart)
### standardPart
Property | Value
--- | ---
IRI | `https://w3id.org/ci#standardPart`
Domain(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](standardYear)
### standardYear
Property | Value
--- | ---
IRI | `https://w3id.org/ci#standardYear`
Domain(s) |[ci:Standard](https://w3id.org/ci#Standard) (c)<br />
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](techspecs)
### tech specs
Property | Value
--- | ---
IRI | `https://w3id.org/ci#techSpecs`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](uniclass)
### uniclass
Property | Value
--- | ---
IRI | `https://w3id.org/ci#uniclass`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](uniformat)
### uniformat
Property | Value
--- | ---
IRI | `https://w3id.org/ci#uniformat`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](unitprice)
### unit price
Property | Value
--- | ---
IRI | `https://w3id.org/ci#unitPrice`
Domain(s) |[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />

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