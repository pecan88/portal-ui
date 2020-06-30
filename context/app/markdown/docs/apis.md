# HuBMAP Application Programmer Interfaces (APIs)
Five application programming interfaces (APIs) currently define 
data ingest support: Ingest, UUID, Search & Index, Entity, and Ontology.  Additionally, the HuBMAP portal uses Common Coordinate Framework (CCF) APIs (created by Indiana University TC) and internal transformation APIs (created by Harvard University TC)

### Ingest API
The Ingest API supports writing data and metadata to HuBMAP. It is used when Tissue Mapping Centers (TMCs) contribute data and also to deposit derived data resulting from the execution of pipelines.
- [GitHub](https://github.com/hubmapconsortium/ingest-ui) 
- [Smart API](https://smart-api.info/ui/5a6bea1158d2652743c7a201fdb1c44d)

### UUID API
The Ingest API supports all donor and tissue sample registration and submission of data and collection of provenance information via the Ingest UI. The Ingest UI is a web user interface used by the Tissue Mapping Centers (TMCs) when contributing raw and derived data which result from the execution of pipelines.
- [GitHub](https://github.com/hubmapconsortium/uuid-api)
- Smart API: currently not available

### Search & Index API
The Search & Index API supports searching and reindexing of HuBMAP metadata and data. The /search endpoint returns sets of data entities matching specifi ed queries for Donors, Tissue Samples and Datasets. The /reindex endpoint is used internally to index new and changed entities, this endpoint is not accessible externally, but only from other APIs that create, update or delete entities.
- [GitHub](https://github.com/hubmapconsortium/search-api)
- [Smart API](https://smart-api.info/ui/7aaf02b838022d564da776b03f357158)

### Ontology API
The Ontology API accesses a Neo4j knowledge graph that allows
extensive cross-referencing across biomedical vocabulary systems.
- [GitHub](https://github.com/hubmapconsortium/hubmap-ontology)
- Smart API: currently not available

### Entity API
The Entity API returns information about HuBMAP data entities (Figure 3). 

Examples of Entity endpoints are as follows:s
 - /entities/types: return valid entity types
 - /entities/{identifer}: return specific entities
 - /entities/types/{type_code}: return UUIDs by entity type
 - /entities/{identifier}/provenance: return provenance
   data for entity

**Figure 3.**
![An example HuBMAP entity graph consisting of a donor, organ, blocks, tissue slices, data and derived data from a pipeline. In general, a donor and organ are required in the provenance hierarchy where tissue samples (such as blocks and samples) can be organized based on several different tissue sample types.](https://drive.google.com/file/d/14aAyTItvm3teFB5jUX5TVGRpW4oit99b/view?usp=sharing)

- [GitHub](https://github.com/hubmapconsortium/entity-api) 
- [Smart API](https://smart-api.info/ui/0065e419668f3336a40d1f5ab89c6ba3)



### Common Coordinate Framework (CCF) Registration User Interface (RUI) and Exploration User Interface (EUI) API
A specification and set of web service calls to return information about CCF-mapped data
[GitHub](https://github.com/hubmapconsortium/ccf-data-api)
[Smart API](https://smart-api.info/ui/d1f33c1a75e9dcda984194e4d8cea7d8)

### [Interface transformation API]
[Ilan/Nils/Chuck: insert text here]
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyMzc3MTU4MjUsLTE0ODgyODI4NjQsLT
E5NDE3NTYzODYsLTE2ODk1MTg0MDEsLTE1MTA1Nzc0MDUsNTAw
NzcxNTM4LC00ODU0NDA1NCw0ODYwMDE4NzUsOTc5NzQwMDYwLC
02MDc2MjEyMTUsLTM3NTkzMzE4NiwtMTM0Mzg4MTc5NCw1OTkz
NDUzNCwtMTQxMTUyMDY5MCwxNDA0MDIzODc5LC0xMzYzMjg4Mj
MzLC0yNTE3MjU0MjMsLTExOTcxNTY4NjQsLTU5MjE1MTE2MSw5
MTM4Mjg1NjFdfQ==
-->
