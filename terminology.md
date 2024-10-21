Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# The Construction Terminology (CTERM) Ontology

## Metadata
* **IRI**
  * `http://w3id.org/cterm`
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
  * [http://w3id.org/cr](http://w3id.org/cr)
* **License &amp; Rights**
  * [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
  * &copy; 2024 by DABC, PoliMi
* **Source**
  * [https://linkedbuildingdata.net/ldac2024/files/papers/LDAC2024_Camera_8.pdf](https://linkedbuildingdata.net/ldac2024/files/papers/LDAC2024_Camera_8.pdf)
* **Ontology RDF**
  * RDF ([terminology.ttl](turtle))
### Description
<p>The Construction Terminology (CTERM) Ontology is based on concepts and principles ... </p>

## Table of Contents
1. [Classes](#classes)
1. [Object Properties](#objectproperties)
1. [Named Individuals](#namedindividuals)
1. [Namespaces](#namespaces)
1. [Legend](#legend)


## Overview

**Figure 1:** Ontology overview
## Classes
[Aspect](#Aspect),
[AspectOfEquipment](#AspectOfEquipment),
[AspectOfMaterial](#AspectOfMaterial),
[AspectOfWorkOfConstructionWork](#AspectOfWorkOfConstructionWork),
[AspectOfWorkOfProductWork](#AspectOfWorkOfProductWork),
[AspectOfWorkOfTemporaryWork](#AspectOfWorkOfTemporaryWork),
[Category](#Category),
[Category of equipment](#Categoryofequipment),
[Category of labour](#Categoryoflabour),
[Category of material](#Categoryofmaterial),
[CategoryOfActivity](#CategoryOfActivity),
[CategoryOfCostComponent](#CategoryOfCostComponent),
[CategoryOfWorkOfConstructionWork](#CategoryOfWorkOfConstructionWork),
[CategoryOfWorkOfProductWork](#CategoryOfWorkOfProductWork),
[CategoryOfWorkOfTemporaryWork](#CategoryOfWorkOfTemporaryWork),
[Family](#Family),
[Family](#Family1),
[Family of equipment](#Familyofequipment),
[Family of labour](#Familyoflabour),
[Family of material](#Familyofmaterial),
[FamilyOfActivity](#FamilyOfActivity),
[FamilyOfCostComponent](#FamilyOfCostComponent),
[FamilyOfWork](#FamilyOfWork),
[Terminology](#Terminology),
### Family
Property | Value
--- | ---
IRI | `https://w3id.org/ci#Family`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Restrictions |[cterm:hasFamily](https://w3id.org/cterm#hasFamily) (op) **exactly** 1 [ci:Family](https://w3id.org/ci#Family) (c)<br />
### Aspect
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Aspect`
Super-classes |[cterm:Terminology](https://w3id.org/cterm#Terminology) (c)<br />
Restrictions |[cterm:hasAspect](https://w3id.org/cterm#hasAspect) (op) **max** 5 [cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
Sub-classes |[cterm:AspectOfMaterial](https://w3id.org/cterm#AspectOfMaterial) (c)<br />[cterm:AspectOfEquipment](https://w3id.org/cterm#AspectOfEquipment) (c)<br />[cterm:AspectOfWorkOfProductWork](https://w3id.org/cterm#AspectOfWorkOfProductWork) (c)<br />[cterm:AspectOfWorkOfTemporaryWork](https://w3id.org/cterm#AspectOfWorkOfTemporaryWork) (c)<br />[cterm:AspectOfWorkOfConstructionWork](https://w3id.org/cterm#AspectOfWorkOfConstructionWork) (c)<br />
In range of |[cterm:hasAspect](https://w3id.org/cterm#hasAspect) (op)<br />
### AspectOfEquipment
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#AspectOfEquipment`
Super-classes |[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
### AspectOfMaterial
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#AspectOfMaterial`
Super-classes |[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
### AspectOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#AspectOfWorkOfConstructionWork`
Super-classes |[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
### AspectOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#AspectOfWorkOfProductWork`
Super-classes |[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
### AspectOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#AspectOfWorkOfTemporaryWork`
Super-classes |[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
### Category
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Category`
Super-classes |[cterm:Terminology](https://w3id.org/cterm#Terminology) (c)<br />
Restrictions |[cterm:hasCategory](https://w3id.org/cterm#hasCategory) (op) **exactly** 1 [cterm:Category](https://w3id.org/cterm#Category) (c)<br />
Sub-classes |[cterm:CategoryOfWorkOfConstructionWork](https://w3id.org/cterm#CategoryOfWorkOfConstructionWork) (c)<br />[cterm:CategoryOfMaterial](https://w3id.org/cterm#CategoryOfMaterial) (c)<br />[cterm:CategoryOfLabour](https://w3id.org/cterm#CategoryOfLabour) (c)<br />[cterm:CategoryOfCostComponent](https://w3id.org/cterm#CategoryOfCostComponent) (c)<br />[cterm:CategoryOfActivity](https://w3id.org/cterm#CategoryOfActivity) (c)<br />[cterm:CategoryOfEquipment](https://w3id.org/cterm#CategoryOfEquipment) (c)<br />[cterm:CategoryOfWorkOfProductWork](https://w3id.org/cterm#CategoryOfWorkOfProductWork) (c)<br />[cterm:CategoryOfWorkOfTemporaryWork](https://w3id.org/cterm#CategoryOfWorkOfTemporaryWork) (c)<br />
In range of |[cterm:hasCategory](https://w3id.org/cterm#hasCategory) (op)<br />
### CategoryOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfActivity`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### CategoryOfCostComponent
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfCostComponent`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### Category of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfEquipment`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### Category of labour
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfLabour`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### Category of material
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfMaterial`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### CategoryOfWorkOfConstructionWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfWorkOfConstructionWork`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### CategoryOfWorkOfProductWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfWorkOfProductWork`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### CategoryOfWorkOfTemporaryWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CategoryOfWorkOfTemporaryWork`
Super-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
### Family
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Family`
Super-classes |[cterm:Terminology](https://w3id.org/cterm#Terminology) (c)<br />
Restrictions |[cterm:hasFamily](https://w3id.org/cterm#hasFamily) (op) **exactly** 1 [cterm:Family](https://w3id.org/cterm#Family) (c)<br />
Sub-classes |[cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork) (c)<br />[cterm:FamilyOfActivity](https://w3id.org/cterm#FamilyOfActivity) (c)<br />[cterm:FamilyOfEquipment](https://w3id.org/cterm#FamilyOfEquipment) (c)<br />[cterm:FamilyOfLabour](https://w3id.org/cterm#FamilyOfLabour) (c)<br />[cterm:FamilyOfCostComponent](https://w3id.org/cterm#FamilyOfCostComponent) (c)<br />[cterm:FamilyOfMaterial](https://w3id.org/cterm#FamilyOfMaterial) (c)<br />
In range of |[cterm:hasFamily](https://w3id.org/cterm#hasFamily) (op)<br />
### FamilyOfActivity
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FamilyOfActivity`
Super-classes |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />
### FamilyOfCostComponent
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FamilyOfCostComponent`
Super-classes |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />
### Family of equipment
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FamilyOfEquipment`
Super-classes |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />
### Family of labour
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FamilyOfLabour`
Super-classes |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />
### Family of material
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FamilyOfMaterial`
Super-classes |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />
### FamilyOfWork
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FamilyOfWork`
Super-classes |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />
### Terminology
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Terminology`
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />[cterm:Family](https://w3id.org/cterm#Family) (c)<br />

## Object Properties
[hasCategory](#hasCategory),
[hasAspect](#hasAspect),
[hasCategory](#hasCategory1),
[hasFamily](#hasFamily),
[](hasCategory)
### hasCategory
Property | Value
--- | ---
IRI | `https://w3id.org/cr#hasCategory`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />
Range(s) |[ci:Category](https://w3id.org/ci#Category) (c)<br />
[](hasAspect)
### hasAspect
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#hasAspect`
Domain(s) |[cr:MaterialResource](https://w3id.org/cr#MaterialResource) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />[cr:EquipmentResource](https://w3id.org/cr#EquipmentResource) (c)<br />
Range(s) |[cterm:Aspect](https://w3id.org/cterm#Aspect) (c)<br />
[](hasCategory1)
### hasCategory
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#hasCategory`
Domain(s) |[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />
Range(s) |[cterm:Category](https://w3id.org/cterm#Category) (c)<br />
[](hasFamily)
### hasFamily
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#hasFamily`
Domain(s) |[cr:Resource](https://w3id.org/cr#Resource) (c)<br />[ci:Work](https://w3id.org/ci#Work) (c)<br />[ci:Activity](https://w3id.org/ci#Activity) (c)<br />[ci:CostComponent](https://w3id.org/ci#CostComponent) (c)<br />
Range(s) |[cterm:Family](https://w3id.org/cterm#Family) (c)<br />

## Named Individuals
[Ambiente](#Ambiente),
[Architettura](#Architettura),
[Arredo](#Arredo),
[CivilEngineer](#CivilEngineer),
[Edilizia](#Edilizia),
[ElectricalEngineer](#ElectricalEngineer),
[FireSafety](#FireSafety),
[Infrastrutture](#Infrastrutture),
[IngegneriaIdraulica](#IngegneriaIdraulica),
[Land](#Land),
[MechanicalEngineer](#MechanicalEngineer),
[Modify](#Modify),
[PrefabricatedStructuresForConcrete](#PrefabricatedStructuresForConcrete),
[Production](#Production),
[StructuralEngineer](#StructuralEngineer),
[VerdeEPaesaggio](#VerdeEPaesaggio),
### Architettura <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Architecture`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### CivilEngineer <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#CivilEngineer`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### Edilizia <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Construction`
* **Contributor(s)**
  * [cterm:FamilyOfCostComponent](https://w3id.org/cterm#FamilyOfCostComponent)
### ElectricalEngineer <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#ElectricalEngineer`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### Ambiente <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Environment`
* **Contributor(s)**
  * [cterm:FamilyOfCostComponent](https://w3id.org/cterm#FamilyOfCostComponent)
### FireSafety <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#FireSafety`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### Arredo <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Furniture`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### IngegneriaIdraulica <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#IdraulicEngineer`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### Infrastrutture <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Infrastructure`
* **Contributor(s)**
  * [cterm:FamilyOfCostComponent](https://w3id.org/cterm#FamilyOfCostComponent)
### Land <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Land`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### VerdeEPaesaggio <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Landscape`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### MechanicalEngineer <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#MechanicalEngineer`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### Modify <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Modify`
* **Contributor(s)**
  * [cterm:FamilyOfActivity](https://w3id.org/cterm#FamilyOfActivity)
### PrefabricatedStructuresForConcrete <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#PrefabricatedStructuresForConcrete`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
### Production <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#Production`
* **Contributor(s)**
  * [cterm:FamilyOfActivity](https://w3id.org/cterm#FamilyOfActivity)
### StructuralEngineer <sup>c</sup>
Property | Value
--- | ---
IRI | `https://w3id.org/cterm#StructuralEngineer`
* **Contributor(s)**
  * [cterm:FamilyOfWork](https://w3id.org/cterm#FamilyOfWork)
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