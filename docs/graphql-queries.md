---
id: graphql-queries
title: GraphQL API
sidebar_label: GraphQL API
sidebar_position: 4
---

# GraphQL API Documentation

This section describes the available **GraphQL API queries**, their usage, required parameters, and example responses.

## API Calls

| Query Name | Description |
|------------|-------------|
| **[allManagerProviders](#post-allmanagerproviders)** | Fetches All Manager Providers |
| **[getAuthorities](#post-getauthorities)** | Fetches All Authorities |
| **[getAuthorityById](#post-getauthoritybyid)** | Fetches an Authority by Id |
| **[getAuthorityByPage](#post-getauthoritybypage)** | Fetches a paginated list of Authorities |
| **[getIdentifierById](#post-getidentifierbyid)** | Fetches an Identifier by Id |
| **[getIdentifiers](#post-getidentifiers)** | Fetches All Identifiers |
| **[getIdentifiersByPage](#post-getidentifiersbypage)** | Fetches a paginated list of identifiers |
| **[getMPAById](#post-getmpabyid)** | Fetches a MPA by Id |
| **[getMPAs](#post-getmpas)** | Get All MPA |
| **[getMPAsByPage](#post-getmpasbypage)** | Fetches a paginated list of MPA |
| **[getManagerById](#post-getmanagerbyid)** | Fetches a Manager by Id |
| **[getManagerByPage](#post-getmanagerbypage)** | Fetches a paginated list of Managers |
| **[getManagers](#post-getmanagers)** | Get All Managers |
| **[getPropertiesStackCombined](#post-getpropertiesstackcombined)** | Fetches combined properties from the database. |
| **[getPropertiesStackCombinedById](#post-getpropertiesstackcombinedbyid)** | Fetches a Property Stack Combination by Id |
| **[getPropertiesStackCombinedByLabel](#post-getpropertiesstackcombinedbylabel)** | Fetches a list of combined (static, dynamic) properties by label |
| **[getPropertiesStackCombinedPaged](#post-getpropertiesstackcombinedpaged)** | Fetches a paginated list of the combined (static, dynamic) properties |
| **[getPropertiesStackDynamic](#post-getpropertiesstackdynamic)** | Fetches properties from the database. |
| **[getPropertiesStackDynamicByLabel](#post-getpropertiesstackdynamicbylabel)** | Fetches a list of dynamic properties by label |
| **[getPropertiesStackDynamicPaged](#post-getpropertiesstackdynamicpaged)** | Fetches a paginated list of dynamic properties |
| **[getPropertiesStackStatic](#post-getpropertiesstackstatic)** | Fetches static properties from the database. |
| **[getPropertiesStackStaticByLabel](#post-getpropertiesstackstaticbylabel)** | Fetches a list of static properties by label |
| **[getPropertiesStackStaticPaged](#post-getpropertiesstackstaticpaged)** | Fetches a paginated list of static properties |
| **[getProviderById](#post-getproviderbyid)** | Fetches a Provider by Id |
| **[getProviders](#post-getproviders)** | Get All Providers |
| **[getProvidersByPage](#post-getprovidersbypage)** | Fetches a paginated list of identifiers |
| **[getResolvedIdentifierAuthorities](#post-getresolvedidentifierauthorities)** | Fetches resolved identifier authority  |
| **[getResolvedIdentifierAuthoritiesByLabel](#post-getresolvedidentifierauthoritiesbylabel)** | Fetches a list of resolved identifier authorities by label |
| **[getResolvedIdentifierAuthoritiesPaged](#post-getresolvedidentifierauthoritiespaged)** | Fetches a paginated list of resolved identifier authorities |
| **[getResolvedIdentifierMPAs](#post-getresolvedidentifiermpas)** | Fetch all resolved identifier mpas |
| **[getResolvedIdentifierMPAsByLabel](#post-getresolvedidentifiermpasbylabel)** | Fetches a list of resolved identifier MPAs by label |
| **[getResolvedIdentifierMPAsPaged](#post-getresolvedidentifiermpaspaged)** | Fetches a paginated list of resolved identifier MPAs |
| **[getResolvedIdentifierProviders](#post-getresolvedidentifierproviders)** | Fetch all resolved identifier provider |
| **[getResolvedIdentifierProvidersByLabel](#post-getresolvedidentifierprovidersbylabel)** | Fetches a list of resolved identifier providers by label |
| **[getResolvedIdentifierProvidersPaged](#post-getresolvedidentifierproviderspaged)** | Fetches a paginated list of resolved identifier providers |
| **[getResolvedIdentifierSchemes](#post-getresolvedidentifierschemes)** | Fetch all resolved identifier schemes |
| **[getResolvedIdentifierSchemesByLabel](#post-getresolvedidentifierschemesbylabel)** | Fetches a list of resolved identifier scheme by label |
| **[getResolvedIdentifierSchemesPaged](#post-getresolvedidentifierschemespaged)** | Fetches a paginated list of resolved identifier schemes |
| **[getResolvedIdentifierStack](#post-getresolvedidentifierstack)** | Fetches resolved identifier stack  |
| **[getResolvedIdentifierStackByActor](#post-getresolvedidentifierstackbyactor)** | Fetches a list of resolved identifier stacks by Actor |
| **[getResolvedIdentifierStackById](#post-getresolvedidentifierstackbyid)** | Fetches a Resolved Identifier Stack by Id |
| **[getResolvedIdentifierStackByLabel](#post-getresolvedidentifierstackbylabel)** | Fetches a list of resolved identifier stacks by Label |
| **[getResolvedIdentifierStackByLabelIdentifier](#post-getresolvedidentifierstackbylabelidentifier)** | Fetches a list of resolved identifier stacks by Identifiers Label |
| **[getResolvedIdentifierStackPaged](#post-getresolvedidentifierstackpaged)** | Fetches a paginated list of resolved identifier Stack |
| **[getResolvedIdentifierStandards](#post-getresolvedidentifierstandards)** | Fetches resolved identifier standard  |
| **[getResolvedIdentifierStandardsByLabel](#post-getresolvedidentifierstandardsbylabel)** | Fetches resolved identifier standard from the database by label. |
| **[getResolvedIdentifierStandardsPaged](#post-getresolvedidentifierstandardspaged)** | Fetches a paginated list of resolved identifier standard |
| **[getSchemeById](#post-getschemebyid)** | Fetches a Scheme by Id |
| **[getSchemes](#post-getschemes)** | Get All Schemes |
| **[getStandardById](#post-getstandardbyid)** | Fetches a Standard by Id |
| **[getStandardByPage](#post-getstandardbypage)** | Fetches a paginated list of Standards |
| **[getStandards](#post-getstandards)** | Get All Standards |
| **[managers](#post-managers)** | Fetches All Managers |
| **[searchPropertiesStackCombinedStack](#post-searchpropertiesstackcombinedstack)** | Fetches a list of properties stacks combined by search |
| **[searchResolvedIdentifierStack](#post-searchresolvedidentifierstack)** | Fetches a list of resolved identifier stacks by search |

---

## **[POST]: allManagerProviders**
#### Description
> 📌 Fetches All Manager Providers

### **Input**
```
query allManagerProviders()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  allManagerProviders() {
    id
    identifier
    lastTouch
    lodRelation
    manager
    populatedBy
    provider
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getAuthorities**
#### Description
> 📌 Fetches All Authorities

### **Input**
```
query getAuthorities()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getAuthorities() {
    aUT
    descAuthority
    iDAUT
    labelAuthority
    lastTouch
    lodAUT
    populatedBy
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getAuthorities": [
            {
                "aUT": "ISBN",
                "descAuthority": "Hosted by International ISBN Agency",
                "iDAUT": null,
                "labelAuthority": "International ISBN Agency",
                "lastTouch": "2025-02-04",
                "lodAUT": "pid_graph:00C7B7CF",
                "populatedBy": "0000-0002-0255-5101"
            },
            {
                "aUT": "OCLC",
                "descAuthority": "Hosted by OCLC (Online Computer Library Center)",
                "iDAUT": null,
                "labelAuthority": "OCLC (Online Computer Library Center)",
                "lastTouch": "2025-02-04",
                "lodAUT": "pid_graph:00F7B08C",
                "populatedBy": "0000-0002-0255-5101"
            },
            {
                "aUT": "National or Regional Tax Authorities",
                "descAuthority": "National or Regional Tax Authorities",
                "iDAUT": null,
                "labelAuthority": "National or Regional Tax Authorities",
                "lastTouch": "2025-02-04",
                "lodAUT": "pid_graph:0217054B",
                "populatedBy": "0000-0002-0255-5101"
            }
        ]
    }
}
```

---

## **[POST]: getAuthorityById**
#### Description
> 📌 Fetches an Authority by Id

### **Input**
```
query getAuthorityById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getAuthorityById(id: String) {
    aUT
    descAuthority
    iDAUT
    labelAuthority
    lastTouch
    lodAUT
    populatedBy
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getAuthorityById": {
            "aUT": "ISBN",
            "descAuthority": "Hosted by International ISBN Agency",
            "iDAUT": null,
            "labelAuthority": "International ISBN Agency",
            "lastTouch": "2025-02-04",
            "lodAUT": "pid_graph:00C7B7CF",
            "populatedBy": "0000-0002-0255-5101"
        }
    }
}
```

---

## **[POST]: getAuthorityByPage**
#### Description
> 📌 Fetches a paginated list of Authorities

### **Input**
```
query getAuthorityByPage(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getAuthorityByPage(page: Int, size: Int) {
    aUT
    descAuthority
    iDAUT
    labelAuthority
    lastTouch
    lodAUT
    populatedBy
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getIdentifierById**
#### Description
> 📌 Fetches an Identifier by Id

### **Input**
```
query getIdentifierById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getIdentifierById(id: String) {
    descIdentifier
    iDIDN
    iDN
    labelIdentifier
    lastTouch
    lodIDN
    lodIND_V
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getIdentifierById": {
            "descIdentifier": "Bibliographic reference code for a journal, maintained by Harvard",
            "iDIDN": null,
            "iDN": "BibCode",
            "labelIdentifier": "BibCode",
            "lastTouch": "30/01/2024",
            "lodIDN": "pid_graph:03A715EA1",
            "lodIND_V": null,
            "populatedBy": "0000-0002-0255-5101",
            "startDate": null
        }
    }
}
```

---

## **[POST]: getIdentifiers**
#### Description
> 📌 Fetches All Identifiers

### **Input**
```
query getIdentifiers()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getIdentifiers() {
    descIdentifier
    iDIDN
    iDN
    labelIdentifier
    lastTouch
    lodIDN
    lodIND_V
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getIdentifiers": [
            {
                "descIdentifier": null,
                "iDIDN": null,
                "iDN": "Book ID",
                "labelIdentifier": "Book ID",
                "lastTouch": "30/01/2024",
                "lodIDN": "pid_graph:55673516",
                "lodIND_V": null,
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            },
            {
                "descIdentifier": "No Identifier has been selected or indicated in relation to recommended use, or in other relationships in the Knowledge Base",
                "iDIDN": null,
                "iDN": "Not Applicable",
                "labelIdentifier": "Not Applicable",
                "lastTouch": "30/01/2024",
                "lodIDN": "pid_graph:075D8338X",
                "lodIND_V": null,
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            },
            {
                "descIdentifier": "PubChem BioAssay contains small-molecule and RNAi screening data along with associated annotation information from contributing organizations. BioAssay contains a collection of bioactivity and toxicity data that has greatly supported research in fields such as medicinal chemistry, drug discovery, pharmaceutical genomics and informatics research. As a primary archive, the provenance of all records belongs to the submitter.",
                "iDIDN": null,
                "iDN": "AID",
                "labelIdentifier": "AID",
                "lastTouch": "30/01/2024",
                "lodIDN": "pid_graph:075D8338",
                "lodIND_V": null,
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            }
        ]
    }
}
```

---

## **[POST]: getIdentifiersByPage**
#### Description
> 📌 Fetches a paginated list of identifiers

### **Input**
```
query getIdentifiersByPage(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getIdentifiersByPage(page: Int, size: Int) {
    descIdentifier
    iDIDN
    iDN
    labelIdentifier
    lastTouch
    lodIDN
    lodIND_V
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getMPAById**
#### Description
> 📌 Fetches a MPA by Id

### **Input**
```
query getMPAById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getMPAById(id: String) {
    descMPA
    iDMPA
    labelMPA
    lastTouch
    lodMPA
    mPA
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getMPAById": {
            "descMPA": "Corporation for National Research Initiatives (CNRI) is a not-for-profit organization formed in 1986 to undertake, foster, and promote research in the public interest. Activities center around strategic development of network-based information technologies, providing leadership and funding for information infrastructure research and development.",
            "iDMPA": null,
            "labelMPA": "Corporation for National Research Initiatives (CNRI)",
            "lastTouch": "20-08-2024",
            "lodMPA": "pid_graph:70E2C260",
            "mPA": "CNRI",
            "populatedBy": "0000-0002-0255-5101",
            "startDate": null
        }
    }
}
```

---

## **[POST]: getMPAs**
#### Description
> 📌 Get All MPA

### **Input**
```
query getMPAs()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getMPAs() {
    descMPA
    iDMPA
    labelMPA
    lastTouch
    lodMPA
    mPA
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getMPAs": [
            {
                "descMPA": "Multi-Provider Agencies are only applicable for some Providers linked to DONA.",
                "iDMPA": null,
                "labelMPA": "Not Applicable",
                "lastTouch": "22-01-2025",
                "lodMPA": "pid_graph:98714B4C1",
                "mPA": "N/A",
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            },
            {
                "descMPA": "Corporation for National Research Initiatives (CNRI) is a not-for-profit organization formed in 1986 to undertake, foster, and promote research in the public interest. Activities center around strategic development of network-based information technologies, providing leadership and funding for information infrastructure research and development.",
                "iDMPA": null,
                "labelMPA": "Corporation for National Research Initiatives (CNRI)",
                "lastTouch": "20-08-2024",
                "lodMPA": "pid_graph:70E2C260",
                "mPA": "CNRI",
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            },
            {
                "descMPA": "ePIC was founded in 2009 by a consortium of European partners in order to provide PID services for the European Research Community, based on the handle system",
                "iDMPA": null,
                "labelMPA": "PID Consortium",
                "lastTouch": "20-08-2024",
                "lodMPA": "pid_graph:28A16295",
                "mPA": "ePIC",
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            }
        ]
    }
}
```

---

## **[POST]: getMPAsByPage**
#### Description
> 📌 Fetches a paginated list of MPA

### **Input**
```
query getMPAsByPage(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getMPAsByPage(page: Int, size: Int) {
    descMPA
    iDMPA
    labelMPA
    lastTouch
    lodMPA
    mPA
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getManagerById**
#### Description
> 📌 Fetches a Manager by Id

### **Input**
```
query getManagerById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getManagerById(id: String) {
    certification
    country
    descManager
    labelManager
    lastTouch
    lodMAN
    lodMAN_V
    mAN
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getManagerById": {
            "certification": null,
            "country": null,
            "descManager": null,
            "labelManager": "<intR>²Dok[§]",
            "lastTouch": "14-01-2025",
            "lodMAN": "pid_graph:2FBC5B5F",
            "lodMAN_V": null,
            "mAN": null,
            "populatedBy": "0009-0006-1756-5317",
            "startDate": null
        }
    }
}
```

---

## **[POST]: getManagerByPage**
#### Description
> 📌 Fetches a paginated list of Managers

### **Input**
```
query getManagerByPage(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getManagerByPage(page: Int, size: Int) {
    certification
    country
    descManager
    labelManager
    lastTouch
    lodMAN
    lodMAN_V
    mAN
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getManagers**
#### Description
> 📌 Get All Managers

### **Input**
```
query getManagers()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getManagers() {
    certification
    country
    descManager
    labelManager
    lastTouch
    lodMAN
    lodMAN_V
    mAN
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getManagers": [
            {
                "certification": null,
                "country": null,
                "descManager": null,
                "labelManager": "]a[repository",
                "lastTouch": "30-08-2024",
                "lodMAN": "pid_graph: 2FBE5E8A3",
                "lodMAN_V": null,
                "mAN": null,
                "populatedBy": "0009-0006-1756-5317",
                "startDate": "2018-12-31T23:00:00Z"
            },
            {
                "certification": null,
                "country": null,
                "descManager": null,
                "labelManager": "<intR>²Dok[§]",
                "lastTouch": "14-01-2025",
                "lodMAN": "pid_graph:2FBC5B5F",
                "lodMAN_V": null,
                "mAN": null,
                "populatedBy": "0009-0006-1756-5317",
                "startDate": null
            },
            {
                "certification": null,
                "country": null,
                "descManager": null,
                "labelManager": "<odesi>",
                "lastTouch": "14-01-2025",
                "lodMAN": "pid_graph:C49FF22D",
                "lodMAN_V": null,
                "mAN": null,
                "populatedBy": "0009-0006-1756-5317",
                "startDate": null
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackCombined**
#### Description
> 📌 Fetches combined properties from the database.

### **Input**
```
query getPropertiesStackCombined()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackCombined() {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackCombined": [
            {
                "labelProperty": "Globally Unique",
                "lodIDN": "pid_graph:C454BB2B",
                "lodRelation": "hasProperty",
                "value": "No"
            },
            {
                "labelProperty": "Disciplinary",
                "lodIDN": "pid_graph:C6B514CF",
                "lodRelation": "hasProperty",
                "value": "Generic"
            },
            {
                "labelProperty": "Identifier Type",
                "lodIDN": "pid_graph:0E85921A",
                "lodRelation": "hasProperty",
                "value": "Allocated"
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackCombinedById**
#### Description
> 📌 Fetches a Property Stack Combination by Id

### **Input**
```
query getPropertiesStackCombinedById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackCombinedById(id: String) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackCombinedById": {
            "labelProperty": "Managers",
            "lodIDN": "pid_graph:D9D0AD30",
            "lodRelation": "hasProperty",
            "value": "1"
        }
    }
}
```

---

## **[POST]: getPropertiesStackCombinedByLabel**
#### Description
> 📌 Fetches a list of combined (static, dynamic) properties by label

### **Input**
```
query getPropertiesStackCombinedByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackCombinedByLabel(label: String) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackCombinedByLabel": [
            {
                "labelProperty": "Status",
                "lodIDN": "pid_graph:4A58E440",
                "lodRelation": "hasProperty",
                "value": "Established"
            },
            {
                "labelProperty": "Status",
                "lodIDN": "pid_graph:03A715EA",
                "lodRelation": "hasProperty",
                "value": "Established"
            },
            {
                "labelProperty": "Status",
                "lodIDN": "pid_graph:B7EB7BAA",
                "lodRelation": "hasProperty",
                "value": "Established"
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackCombinedPaged**
#### Description
> 📌 Fetches a paginated list of the combined (static, dynamic) properties

### **Input**
```
query getPropertiesStackCombinedPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackCombinedPaged(page: Int, size: Int) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getPropertiesStackDynamic**
#### Description
> 📌 Fetches properties from the database.

### **Input**
```
query getPropertiesStackDynamic()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackDynamic() {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackDynamic": [
            {
                "labelProperty": "Managers",
                "lodIDN": "pid_graph:4EA08A5A",
                "lodRelation": "hasProperty",
                "value": "1"
            },
            {
                "labelProperty": "Managers",
                "lodIDN": "pid_graph:50E7B5FE",
                "lodRelation": "hasProperty",
                "value": "1"
            },
            {
                "labelProperty": "Managers",
                "lodIDN": "pid_graph:52184C71",
                "lodRelation": "hasProperty",
                "value": "1"
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackDynamicByLabel**
#### Description
> 📌 Fetches a list of dynamic properties by label

### **Input**
```
query getPropertiesStackDynamicByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackDynamicByLabel(label: String) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackDynamicByLabel": [
            {
                "labelProperty": "Managers",
                "lodIDN": "pid_graph:4EA08A5A",
                "lodRelation": "hasProperty",
                "value": "1"
            },
            {
                "labelProperty": "Managers",
                "lodIDN": "pid_graph:50E7B5FE",
                "lodRelation": "hasProperty",
                "value": "1"
            },
            {
                "labelProperty": "Managers",
                "lodIDN": "pid_graph:52184C71",
                "lodRelation": "hasProperty",
                "value": "1"
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackDynamicPaged**
#### Description
> 📌 Fetches a paginated list of dynamic properties

### **Input**
```
query getPropertiesStackDynamicPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackDynamicPaged(page: Int, size: Int) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getPropertiesStackStatic**
#### Description
> 📌 Fetches static properties from the database.

### **Input**
```
query getPropertiesStackStatic()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackStatic() {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackStatic": [
            {
                "labelProperty": "Resolution Topology",
                "lodIDN": "pid_graph:016841FF",
                "lodRelation": "hasProperty",
                "value": "Resolver"
            },
            {
                "labelProperty": "Resolution Topology",
                "lodIDN": "pid_graph:016841FF",
                "lodRelation": "hasProperty",
                "value": "Resolver"
            },
            {
                "labelProperty": "Resolution Topology",
                "lodIDN": "pid_graph:016841FF",
                "lodRelation": "hasProperty",
                "value": "Resolver"
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackStaticByLabel**
#### Description
> 📌 Fetches a list of static properties by label

### **Input**
```
query getPropertiesStackStaticByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackStaticByLabel(label: String) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getPropertiesStackStaticByLabel": [
            {
                "labelProperty": "Resolution Topology",
                "lodIDN": "pid_graph:016841FF",
                "lodRelation": "hasProperty",
                "value": "Resolver"
            },
            {
                "labelProperty": "Resolution Topology",
                "lodIDN": "pid_graph:025992EB",
                "lodRelation": "hasProperty",
                "value": "Resolver"
            },
            {
                "labelProperty": "Resolution Topology",
                "lodIDN": "pid_graph:03A715EA",
                "lodRelation": "hasProperty",
                "value": "Resolver"
            }
        ]
    }
}
```

---

## **[POST]: getPropertiesStackStaticPaged**
#### Description
> 📌 Fetches a paginated list of static properties

### **Input**
```
query getPropertiesStackStaticPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getPropertiesStackStaticPaged(page: Int, size: Int) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getProviderById**
#### Description
> 📌 Fetches a Provider by Id

### **Input**
```
query getProviderById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getProviderById(id: String) {
    country
    descProvider
    iDPRV
    labelProvider
    lastTouch
    lodPRV
    lodPRV_V
    lodTPR
    pRV
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getProviderById": {
            "country": "AUS",
            "descProvider": "Sample holders and curators affiliated with Australian research organisations that do not offer their own IGSN minting service",
            "iDPRV": null,
            "labelProvider": "Australian Research Data Commons (ARDC)",
            "lastTouch": "2024-08-18",
            "lodPRV": "pid_graph:3C391CE0",
            "lodPRV_V": null,
            "lodTPR": "pid_graph:DB893DE8",
            "pRV": null,
            "populatedBy": "0000-0002-0255-5101",
            "startDate": null
        }
    }
}
```

---

## **[POST]: getProviders**
#### Description
> 📌 Get All Providers

### **Input**
```
query getProviders()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getProviders() {
    country
    descProvider
    iDPRV
    labelProvider
    lastTouch
    lodPRV
    lodPRV_V
    lodTPR
    pRV
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getProviders": [
            {
                "country": "AUS",
                "descProvider": null,
                "iDPRV": null,
                "labelProvider": "RAID Australia",
                "lastTouch": "2025-01-19",
                "lodPRV": "pid_graph:6AA27949",
                "lodPRV_V": null,
                "lodTPR": "pid_graph:DB893DE8",
                "pRV": null,
                "populatedBy": "0009-0006-1756-5317",
                "startDate": null
            },
            {
                "country": "AUS",
                "descProvider": "Sample holders and curators affiliated with Australian research organisations that do not offer their own IGSN minting service",
                "iDPRV": null,
                "labelProvider": "Australian Research Data Commons (ARDC)",
                "lastTouch": "2024-08-18",
                "lodPRV": "pid_graph:3C391CE0",
                "lodPRV_V": null,
                "lodTPR": "pid_graph:DB893DE8",
                "pRV": null,
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            },
            {
                "country": "AUS",
                "descProvider": "Organization facilities and staff",
                "iDPRV": null,
                "labelProvider": "Commonwealth Scientific and Industrial Research Organisation (CSIRO)",
                "lastTouch": "2024-08-18",
                "lodPRV": "pid_graph:F46811F9",
                "lodPRV_V": null,
                "lodTPR": "pid_graph:DB893DE8",
                "pRV": null,
                "populatedBy": "0000-0002-0255-5101",
                "startDate": null
            }
        ]
    }
}
```

---

## **[POST]: getProvidersByPage**
#### Description
> 📌 Fetches a paginated list of identifiers

### **Input**
```
query getProvidersByPage(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getProvidersByPage(page: Int, size: Int) {
    country
    descProvider
    iDPRV
    labelProvider
    lastTouch
    lodPRV
    lodPRV_V
    lodTPR
    pRV
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getResolvedIdentifierAuthorities**
#### Description
> 📌 Fetches resolved identifier authority 

### **Input**
```
query getResolvedIdentifierAuthorities()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierAuthorities() {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierAuthorities": [
            {
                "actor": "Authority",
                "label": "GS1",
                "labelIdentifier": "EAN13",
                "lod": "pid_graph:DE972BC0",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:025992EB"
            },
            {
                "actor": "Authority",
                "label": "arXiv.org",
                "labelIdentifier": "arXiv",
                "lod": "pid_graph:F34A3E3D8",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:03A715EA"
            },
            {
                "actor": "Authority",
                "label": "NASA Astrophysics Data System (ADS)",
                "labelIdentifier": "BibCode",
                "lod": "pid_graph:A84EFB6C",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:03A715EA1"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierAuthoritiesByLabel**
#### Description
> 📌 Fetches a list of resolved identifier authorities by label

### **Input**
```
query getResolvedIdentifierAuthoritiesByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierAuthoritiesByLabel(label: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierAuthoritiesByLabel": [
            {
                "actor": "Authority",
                "label": "DONA",
                "labelIdentifier": "RAID",
                "lod": "pid_graph:7F908AED",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:0D27745F"
            },
            {
                "actor": "Authority",
                "label": "DONA",
                "labelIdentifier": "IGSN",
                "lod": "pid_graph:7F908AED",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:0E85921A"
            },
            {
                "actor": "Authority",
                "label": "DONA",
                "labelIdentifier": "PIDINST",
                "lod": "pid_graph:7F908AED",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:152D52742"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierAuthoritiesPaged**
#### Description
> 📌 Fetches a paginated list of resolved identifier authorities

### **Input**
```
query getResolvedIdentifierAuthoritiesPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierAuthoritiesPaged(page: Int, size: Int) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getResolvedIdentifierMPAs**
#### Description
> 📌 Fetch all resolved identifier mpas

### **Input**
```
query getResolvedIdentifierMPAs()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierMPAs() {
    actor
    labelIdentifier
    labelMPA
    lodAct
    lodIdn
    lodMPA
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierMPAs": [
            {
                "actor": "MPA",
                "labelIdentifier": "EAN13",
                "labelMPA": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIdn": "pid_graph:025992EB",
                "lodMPA": null
            },
            {
                "actor": "MPA",
                "labelIdentifier": "arXiv",
                "labelMPA": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIdn": "pid_graph:03A715EA",
                "lodMPA": null
            },
            {
                "actor": "MPA",
                "labelIdentifier": "BibCode",
                "labelMPA": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIdn": "pid_graph:03A715EA1",
                "lodMPA": null
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierMPAsByLabel**
#### Description
> 📌 Fetches a list of resolved identifier MPAs by label

### **Input**
```
query getResolvedIdentifierMPAsByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierMPAsByLabel(label: String) {
    actor
    labelIdentifier
    labelMPA
    lodAct
    lodIdn
    lodMPA
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierMPAsByLabel": [
            {
                "actor": "MPA",
                "labelIdentifier": "ORCID",
                "labelMPA": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIdn": "pid_graph:152D5274",
                "lodMPA": null
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierMPAsPaged**
#### Description
> 📌 Fetches a paginated list of resolved identifier MPAs

### **Input**
```
query getResolvedIdentifierMPAsPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierMPAsPaged(page: Int, size: Int) {
    actor
    labelIdentifier
    labelMPA
    lodAct
    lodIdn
    lodMPA
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getResolvedIdentifierProviders**
#### Description
> 📌 Fetch all resolved identifier provider

### **Input**
```
query getResolvedIdentifierProviders()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierProviders() {
    actor
    labelIdentifier
    labelProvider
    lodAct
    lodIdn
    lodPrv
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierProviders": [
            {
                "actor": "Provider",
                "labelIdentifier": "LCCN",
                "labelProvider": null,
                "lodAct": "pid_graph:E92B9B49",
                "lodIdn": "pid_graph:016841FF",
                "lodPrv": null
            },
            {
                "actor": "Provider",
                "labelIdentifier": "EAN13",
                "labelProvider": "International Article Number (EAN)",
                "lodAct": "pid_graph:E92B9B49",
                "lodIdn": "pid_graph:025992EB",
                "lodPrv": "pid_graph:34072556"
            },
            {
                "actor": "Provider",
                "labelIdentifier": "arXiv",
                "labelProvider": "arXiv.org",
                "lodAct": "pid_graph:E92B9B49",
                "lodIdn": "pid_graph:03A715EA",
                "lodPrv": "pid_graph:78C5DD5E"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierProvidersByLabel**
#### Description
> 📌 Fetches a list of resolved identifier providers by label

### **Input**
```
query getResolvedIdentifierProvidersByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierProvidersByLabel(label: String) {
    actor
    labelIdentifier
    labelProvider
    lodAct
    lodIdn
    lodPrv
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierProvidersByLabel": [
            {
                "actor": "Provider",
                "labelIdentifier": "arXiv",
                "labelProvider": "arXiv.org",
                "lodAct": "pid_graph:E92B9B49",
                "lodIdn": "pid_graph:03A715EA",
                "lodPrv": "pid_graph:78C5DD5E"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierProvidersPaged**
#### Description
> 📌 Fetches a paginated list of resolved identifier providers

### **Input**
```
query getResolvedIdentifierProvidersPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierProvidersPaged(page: Int, size: Int) {
    actor
    labelIdentifier
    labelProvider
    lodAct
    lodIdn
    lodPrv
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getResolvedIdentifierSchemes**
#### Description
> 📌 Fetch all resolved identifier schemes

### **Input**
```
query getResolvedIdentifierSchemes()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierSchemes() {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierSchemes": [
            {
                "actor": "Scheme",
                "label": "LCCN Scheme",
                "labelIdentifier": "LCCN",
                "lod": "pid_graph:3419AB81",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:016841FF"
            },
            {
                "actor": "Scheme",
                "label": "European Article Number",
                "labelIdentifier": "EAN13",
                "lod": "pid_graph:DA568C41",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:025992EB"
            },
            {
                "actor": "Scheme",
                "label": "ArXiv Scheme",
                "labelIdentifier": "arXiv",
                "lod": "pid_graph:D1879DD9",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:03A715EA"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierSchemesByLabel**
#### Description
> 📌 Fetches a list of resolved identifier scheme by label

### **Input**
```
query getResolvedIdentifierSchemesByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierSchemesByLabel(label: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierSchemesByLabel": [
            {
                "actor": "Scheme",
                "label": "URN:NBN",
                "labelIdentifier": "URN:NBN:CZ",
                "lod": "pid_graph:W95785C8E",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:369FA36F"
            },
            {
                "actor": "Scheme",
                "label": "URN:NBN",
                "labelIdentifier": "URN:NBN:IT",
                "lod": "pid_graph:W95785C8E",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:4EA08A5A"
            },
            {
                "actor": "Scheme",
                "label": "URN:NBN",
                "labelIdentifier": "URN:NBN:AT",
                "lod": "pid_graph:W95785C8E",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:68ADD24A"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierSchemesPaged**
#### Description
> 📌 Fetches a paginated list of resolved identifier schemes

### **Input**
```
query getResolvedIdentifierSchemesPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierSchemesPaged(page: Int, size: Int) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getResolvedIdentifierStack**
#### Description
> 📌 Fetches resolved identifier stack 

### **Input**
```
query getResolvedIdentifierStack()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStack() {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStack": [
            {
                "actor": "MPA",
                "label": null,
                "labelIdentifier": "AID",
                "lod": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIDN": "pid_graph:075D8338"
            },
            {
                "actor": "MPA",
                "label": null,
                "labelIdentifier": "AID",
                "lod": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIDN": "pid_graph:075D8338"
            },
            {
                "actor": "MPA",
                "label": null,
                "labelIdentifier": "AID",
                "lod": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIDN": "pid_graph:075D8338"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierStackByActor**
#### Description
> 📌 Fetches a list of resolved identifier stacks by Actor

### **Input**
```
query getResolvedIdentifierStackByActor(actor: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStackByActor(actor: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStackByActor": [
            {
                "actor": "Authority",
                "label": "NCBI",
                "labelIdentifier": "AID",
                "lod": "pid_graph:E1BEACFF",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:075D8338"
            },
            {
                "actor": "Authority",
                "label": "ARK Alliance Technical Working Group",
                "labelIdentifier": "ARK",
                "lod": "pid_graph:F34A3E3D5",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:15BEDB40"
            },
            {
                "actor": "Authority",
                "label": "arXiv.org",
                "labelIdentifier": "arXiv",
                "lod": "pid_graph:F34A3E3D8",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:03A715EA"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierStackById**
#### Description
> 📌 Fetches a Resolved Identifier Stack by Id

### **Input**
```
query getResolvedIdentifierStackById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStackById(id: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStackById": {
            "actor": "MPA",
            "label": "Corporation for National Research Initiatives (CNRI)",
            "labelIdentifier": "DCO-ID",
            "lod": "pid_graph:70E2C260",
            "lodAct": "pid_graph:7835EF43",
            "lodIDN": "pid_graph:998B7874"
        }
    }
}
```

---

## **[POST]: getResolvedIdentifierStackByLabel**
#### Description
> 📌 Fetches a list of resolved identifier stacks by Label

### **Input**
```
query getResolvedIdentifierStackByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStackByLabel(label: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStackByLabel": [
            {
                "actor": "Authority",
                "label": "DONA",
                "labelIdentifier": "DCO-ID",
                "lod": "pid_graph:7F908AED",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:998B7874"
            },
            {
                "actor": "Authority",
                "label": "DONA",
                "labelIdentifier": "DOI",
                "lod": "pid_graph:7F908AED",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:3E6F3EE6"
            },
            {
                "actor": "Authority",
                "label": "DONA",
                "labelIdentifier": "DOI: Crossref",
                "lod": "pid_graph:7F908AED",
                "lodAct": "pid_graph:1A718108",
                "lodIDN": "pid_graph:3E6F3EE61"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierStackByLabelIdentifier**
#### Description
> 📌 Fetches a list of resolved identifier stacks by Identifiers Label

### **Input**
```
query getResolvedIdentifierStackByLabelIdentifier(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStackByLabelIdentifier(label: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStackByLabelIdentifier": [
            {
                "actor": "Scheme",
                "label": "Digital Object Identifier",
                "labelIdentifier": "DOI",
                "lod": "pid_graph:12A44A8C",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:3E6F3EE6"
            },
            {
                "actor": "Scheme",
                "label": "Digital Object Identifier",
                "labelIdentifier": "DOI",
                "lod": "pid_graph:12A44A8C",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:3E6F3EE6"
            },
            {
                "actor": "Scheme",
                "label": "Digital Object Identifier",
                "labelIdentifier": "DOI",
                "lod": "pid_graph:12A44A8C",
                "lodAct": "pid_graph:0E00C332",
                "lodIDN": "pid_graph:3E6F3EE6"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierStackPaged**
#### Description
> 📌 Fetches a paginated list of resolved identifier Stack

### **Input**
```
query getResolvedIdentifierStackPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStackPaged(page: Int, size: Int) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getResolvedIdentifierStandards**
#### Description
> 📌 Fetches resolved identifier standard 

### **Input**
```
query getResolvedIdentifierStandards()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStandards() {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStandards": [
            {
                "actor": "Standard",
                "label": "Structure of the LC Control Number",
                "labelIdentifier": "LCCN",
                "lod": "pid_graph:37CF6252",
                "lodAct": "(to be registered)",
                "lodIDN": "pid_graph:016841FF"
            },
            {
                "actor": "Standard",
                "label": "GS1 General Specifications",
                "labelIdentifier": "EAN13",
                "lod": "pid_graph:Z90BFDFCF",
                "lodAct": "(to be registered)",
                "lodIDN": "pid_graph:025992EB"
            },
            {
                "actor": "Standard",
                "label": "arXiv Internal Standard",
                "labelIdentifier": "arXiv",
                "lod": "pid_graph:FCDAACDB",
                "lodAct": "(to be registered)",
                "lodIDN": "pid_graph:03A715EA"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierStandardsByLabel**
#### Description
> 📌 Fetches resolved identifier standard from the database by label.

### **Input**
```
query getResolvedIdentifierStandardsByLabel(label: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStandardsByLabel(label: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getResolvedIdentifierStandardsByLabel": [
            {
                "actor": "Standard",
                "label": "Bibcode Published Schema",
                "labelIdentifier": "BibCode",
                "lod": "pid_graph:A6DD5C860",
                "lodAct": "(to be registered)",
                "lodIDN": "pid_graph:03A715EA1"
            }
        ]
    }
}
```

---

## **[POST]: getResolvedIdentifierStandardsPaged**
#### Description
> 📌 Fetches a paginated list of resolved identifier standard

### **Input**
```
query getResolvedIdentifierStandardsPaged(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getResolvedIdentifierStandardsPaged(page: Int, size: Int) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getSchemeById**
#### Description
> 📌 Fetches a Scheme by Id

### **Input**
```
query getSchemeById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getSchemeById(id: String) {
    descScheme
    iDSCH
    labelScheme
    lastTouch
    lodSCH
    lodSCH_V
    lodTSC
    populatedBy
    sCH
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getSchemeById": {
            "descScheme": "The dbGaP ID (Database of Genotypes and Phenotypes Identifier) is a unique alphanumeric identifier assigned to studies, datasets, and other entities within the NCBI’s dbGaP database. The dbGaP ID scheme typically consists of a prefix followed by a numeric",
            "iDSCH": null,
            "labelScheme": "dbGaP Scheme",
            "lastTouch": "12/12/2024",
            "lodSCH": "pid_graph:466E3789",
            "lodSCH_V": null,
            "lodTSC": "Internal",
            "populatedBy": "0000-0002-0255-5101",
            "sCH": null,
            "startDate": null
        }
    }
}
```

---

## **[POST]: getSchemes**
#### Description
> 📌 Get All Schemes

### **Input**
```
query getSchemes()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getSchemes() {
    descScheme
    iDSCH
    labelScheme
    lastTouch
    lodSCH
    lodSCH_V
    lodTSC
    populatedBy
    sCH
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getSchemes": [
            {
                "descScheme": "The AID is an internal scheme specific to the PubChem database.",
                "iDSCH": null,
                "labelScheme": "AID Scheme",
                "lastTouch": "12/12/2024",
                "lodSCH": "pid_graph:30823C63",
                "lodSCH_V": null,
                "lodTSC": "Internal",
                "populatedBy": "0000-0002-0255-5101",
                "sCH": null,
                "startDate": null
            },
            {
                "descScheme": "Unique number used to identify archival collection locations within the UK and key global repositories holding collections relating to British history",
                "iDSCH": null,
                "labelScheme": "ARCHON Code",
                "lastTouch": "12/12/2024",
                "lodSCH": "pid_graph:4472D271",
                "lodSCH_V": null,
                "lodTSC": "Internal",
                "populatedBy": "0000-0002-0255-5101",
                "sCH": null,
                "startDate": null
            },
            {
                "descScheme": "ARK Identifier Scheme",
                "iDSCH": null,
                "labelScheme": "ARK Scheme",
                "lastTouch": "12/12/2024",
                "lodSCH": "pid_graph:D662BC92",
                "lodSCH_V": null,
                "lodTSC": "Published",
                "populatedBy": "0000-0002-0255-5101",
                "sCH": null,
                "startDate": null
            }
        ]
    }
}
```

---

## **[POST]: getStandardById**
#### Description
> 📌 Fetches a Standard by Id

### **Input**
```
query getStandardById(id: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getStandardById(id: String) {
    descStandard
    iDSTD
    labelStandard
    lastTouch
    lodSTD
    lodSTD_V
    lodTST
    populatedBy
    sTD
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getStandardById": {
            "descStandard": "The arXiv identifier does not conform to the DOI standard or any other ISO standards for unique identifiers. It is a custom system developed specifically for the arXiv repository.",
            "iDSTD": null,
            "labelStandard": "arXiv Internal Standard",
            "lastTouch": "12/12/2024",
            "lodSTD": "pid_graph:FCDAACDB",
            "lodSTD_V": null,
            "lodTST": "Internal",
            "populatedBy": "0000-0002-0255-5101",
            "sTD": null,
            "startDate": null
        }
    }
}
```

---

## **[POST]: getStandardByPage**
#### Description
> 📌 Fetches a paginated list of Standards

### **Input**
```
query getStandardByPage(page: Int, size: Int)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getStandardByPage(page: Int, size: Int) {
    descStandard
    iDSTD
    labelStandard
    lastTouch
    lodSTD
    lodSTD_V
    lodTST
    populatedBy
    sTD
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
 Example not provided 
```

---

## **[POST]: getStandards**
#### Description
> 📌 Get All Standards

### **Input**
```
query getStandards()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  getStandards() {
    descStandard
    iDSTD
    labelStandard
    lastTouch
    lodSTD
    lodSTD_V
    lodTST
    populatedBy
    sTD
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "getStandards": [
            {
                "descStandard": "The SRA accession system is part of the larger Bioinformatics Data Management Systems used by the NCBI to manage, archive, and share genomic sequence data.",
                "iDSTD": null,
                "labelStandard": "SRA Scheme Internal Standard",
                "lastTouch": "12/12/2024",
                "lodSTD": "pid_graph:03C5D7F5",
                "lodSTD_V": null,
                "lodTST": "Internal",
                "populatedBy": "0000-0002-0255-5101",
                "sTD": null,
                "startDate": null
            },
            {
                "descStandard": "No specific standard is known for this identifier. If yiou have information on the standard, please contact us via the helpdesk button (bottom right)",
                "iDSTD": null,
                "labelStandard": "None",
                "lastTouch": "12/12/2024",
                "lodSTD": "pid_graph:03C5D7F5X",
                "lodSTD_V": null,
                "lodTST": "None",
                "populatedBy": "0000-0002-0255-5101",
                "sTD": null,
                "startDate": null
            },
            {
                "descStandard": "The Genome ID is  an internal identifier specific to the database or system in which it is used, such as NCBI’s Genome Database. The system for assigning GI numbers was developed by NCBI to manage the large amount of sequence data in its repositories, and",
                "iDSTD": null,
                "labelStandard": "Genome ID Standard",
                "lastTouch": "12/12/2024",
                "lodSTD": "pid_graph:08650BA9",
                "lodSTD_V": null,
                "lodTST": "Internal",
                "populatedBy": "0000-0002-0255-5101",
                "sTD": null,
                "startDate": null
            }
        ]
    }
}
```

---

## **[POST]: managers**
#### Description
> 📌 Fetches All Managers

### **Input**
```
query managers()
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  managers() {
    certification
    country
    descManager
    labelManager
    lastTouch
    lodMAN
    lodMAN_V
    mAN
    populatedBy
    startDate
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "errors": [
        {
            "message": "System error",
            "locations": [
                {
                    "line": 2,
                    "column": 3
                }
            ],
            "path": [
                "managers"
            ],
            "extensions": {
                "classification": "DataFetchingException"
            }
        }
    ],
    "data": {
        "managers": null
    }
}
```

---

## **[POST]: searchPropertiesStackCombinedStack**
#### Description
> 📌 Fetches a list of properties stacks combined by search

### **Input**
```
query searchPropertiesStackCombinedStack(search: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  searchPropertiesStackCombinedStack(search: String) {
    labelProperty
    lodIDN
    lodRelation
    value
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "searchPropertiesStackCombinedStack": [
            {
                "labelProperty": "Globally Unique",
                "lodIDN": "pid_graph:C454BB2B",
                "lodRelation": "hasProperty",
                "value": "No"
            },
            {
                "labelProperty": "Disciplinary",
                "lodIDN": "pid_graph:C6B514CF",
                "lodRelation": "hasProperty",
                "value": "Generic"
            },
            {
                "labelProperty": "Identifier Type",
                "lodIDN": "pid_graph:0E85921A",
                "lodRelation": "hasProperty",
                "value": "Allocated"
            }
        ]
    }
}
```

---

## **[POST]: searchResolvedIdentifierStack**
#### Description
> 📌 Fetches a list of resolved identifier stacks by search

### **Input**
```
query searchResolvedIdentifierStack(search: String)
```

#### Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer YOUR_ACCESS_TOKEN"
}
```

#### **Query**
```graphql
query {
  searchResolvedIdentifierStack(search: String) {
    actor
    label
    labelIdentifier
    lod
    lodAct
    lodIDN
  }
}
```

### **Response**
#### **Headers**
```
Status: 200 OK
```

#### **Response body:**

```json
{
    "data": {
        "searchResolvedIdentifierStack": [
            {
                "actor": "MPA",
                "label": null,
                "labelIdentifier": "AID",
                "lod": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIDN": "pid_graph:075D8338"
            },
            {
                "actor": "MPA",
                "label": null,
                "labelIdentifier": "ARK",
                "lod": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIDN": "pid_graph:15BEDB40"
            },
            {
                "actor": "MPA",
                "label": null,
                "labelIdentifier": "arXiv",
                "lod": null,
                "lodAct": "pid_graph:7835EF43",
                "lodIDN": "pid_graph:03A715EA"
            }
        ]
    }
}
```

---
