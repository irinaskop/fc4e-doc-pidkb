---
title: "Identifiers"
sidebar_position: 3
---
# Identifiers as the Core of the Knowledge Base

Identifiers serve as persistent, unique references to digital or physical objects. The Knowledge Base revolves around the principle that every piece of information is linked to an Identifier either directly or indirectly.  Specifically, Managers can be the issuers (‘minter’) of one or more Identifiers, and of course, an Identifier can be issued by many Managers. This makes Identifiers the fundamental entity in the system. Then as a result a Manager is linked to a specific Provider for a specific Identifier. 


## The Role of Identifiers

An Identifier is a structured piece of information used to uniquely and persistently reference an object.

**Examples:** DOI, ORCID, ISBN, ISSN, ARK, Handle, URN.


| Name    | Description | Example | 
| -------- | ------- | ------- | 
| DOI  | A DOI is a digital identifier of an object, any object — physical, digital, or abstract. DOIs solve a common problem: keeping track of things. Things can be matter, material, content, or activities.   |10.1000/182 | 
| ORCID  | a unique, persistent identifier free of charge to researchers  | 0000-0001-9718-6515 |
| ISBN | An ISBN is an International Standard Book Number. ISBNs were 10 digits in length up to the end of December 2006, but since 1 January 2007 they now always consist of 13 digits. ISBNs are calculated using a specific mathematical formula and include a check digit to validate the number. | 978-92-95055-02-5 |
| ISSN | An International Standard Serial Number (ISSN) is an eight-digit serial number used to uniquely identify a serial publication (periodical), such as a magazine.| 2049-3630|
| ARK |An Archival Resource Key (ARK) is a multi-purpose URL suited to being a persistent identifier for information objects of any type. It is widely used by libraries, data centers, archives, museums, publishers, and government agencies to provide reliable references to scholarly, scientific, and cultural objects. | ark:/67531/metapth346554|
|URN |URNs are globally unique persistent identifiers assigned within defined namespaces so they will be available for a long period of time, even after the resource which they identify ceases to exist or becomes unavailable. | urn:isbn:0451450523 |


Identifiers provide a standardized way of referencing digital and physical resources, ensuring long-term accessibility and data interoperability.

## How Identifiers Are Issued and Managed

- **Managers** (e.g., repositories, institutions) issue and manage Identifiers.
- **Providers** act as intermediaries, enabling Identifier registration, resolution, and governance.
- **Authorities** (e.g., GS1, DataCite) ensure Identifier uniqueness and enforce compliance with governance standards.
- **Schemes & Standards** define how Identifiers are structured and maintained.

## Identifier Properties

Identifiers have potentially many Properties, and the structure allows for an unspecified number of defined **Properties** to be linked to an Identifier. It also allows for efficient storage of varying completeness in the scope of Properties known for an Identifier. 

The Properties are also linked, whenever possible, to well-known definitions - for example by schema.org or Wikidata.

## Identifier Governance and Compliance

- Identifiers are typically backed by a governing Authority that ensures uniqueness and resolvability.
- Standards & Schemes define frameworks for ensuring Identifier integrity.
- Some Identifiers are protocol-based, requiring specific technical infrastructure for resolution (e.g., Handle System, DOI).

## Entities Represented by Identifiers

Identifiers can be used to resolve to and represent one or more well-defined Entities, for example Research Outputs, Researchers, Samples, and many more. There are numerous ontologies and vocabularies for describing the Entities that are in scope in the research landscape, and it is ongoing work to reconcile these. At present, we work with a subset on the basis of need, in other words if an Entity is not referenced, we do not list it.

The source of links between Entities and Identifiers are ‘Case Studies’, which include national PID policies and strategies, desktop research, one or two published community surveys, and AI-supported research. These Case Studies have additional attributes, in the sense that they may recommend, mandate, or anticipate the application of an Identifier for a specific Entity, and that their application scope is either national, regional, or global.


## Special Cases in Identifier Management

- **Identifiers Without a Manager:** Some Identifiers are issued directly by a Provider without a Manager.
- **Generic vs. Specific Identifiers:** Some databases list generic Identifiers (e.g., "DOI" without specifying the Provider), requiring an "Unknown Provider" entry.
- **Identifiers and Their Properties:** Identifiers can have multiple metadata properties, defining attributes, classifications, and additional details.
