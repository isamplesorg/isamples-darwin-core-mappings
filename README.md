# Semantic Mappings of the iSamples Model to the Darwin Core Standard

This repository contains semantic mappings of the iSamples Model to Darwin Core (DWC) and Darwin Core Data Package (DWC DP). Reported mappings adhere to the [Simple Standard for Sharing Ontology Mappings (SSSOM)](https://mapping-commons.github.io/sssom/) specification. 

This repository contains the following semantic mapping sets:
1. [dwc-mappings] iSamples Model (sssom:object_source) and (Simple) Darwin Core (sssom:subject_source) - ***Complete***
2. [dwc-dp-mappings] iSamples Model (sssom:object_source) and the latest version (as of 2025-02-22) Darwin Core DP (sssom:subject_source) - ***Under Review***
   
Each mapping set contains the following files
1. YAML File containing a serialization of the MappingSet object
2. Tab-delimited file containing the mappings block (individual mappings)

## Additional Notes and Resources

| Title | Description | URL |
| -- | -- | -- |
| Sources | Collection of source files for the semantic mappings, which are subsets of the full source for the purposes of semantic mapping  | [https://github.com/ben-norton/isamples-dwc-mappings/tree/main/sources](https://github.com/ben-norton/isamples-dwc-mappings/tree/main/sources) |
| Mapping Resources | A collection of curated web-based resources for Semantic Mapping exercises | [https://github.com/ben-norton/isamples-dwc-mappings/blob/main/resources.md](https://github.com/ben-norton/isamples-dwc-mappings/blob/main/resources.md) |
| Glossary | A tabulated glossary of important semantic mapping terms | [https://github.com/ben-norton/isamples-dwc-mappings/blob/main/glossary.md](https://github.com/ben-norton/isamples-dwc-mappings/blob/main/glossary.md) |

## Approach

### Simplified procedure
1. Conduct Class mapping between the object and subject (see [https://github.com/ben-norton/isamples-dwc-mappings/blob/main/glossary.md](https://github.com/ben-norton/isamples-dwc-mappings/blob/main/glossary.md)
2. When conducting property mappings, only terms belonging to the mapped class are considered. 
Example:
isam:MaterialSampleCuration is a skos:relatedMatch to dwc:MaterialEntity
Object properties that belong to isam:MaterialSampleCuration are mapped to properties belonging to the dwc:MaterialEntity class in the subject vocabulary.
Object properties that belong to isam:Location cannot be mapped to properties in the subject class, dwc:Occurrence because isam:Location cannot be mapped to dwc:Occurrence
Record-level terms in Darwin Core are an exception. Generalized terms such as dcterms:rightsHolder can be mapped to any term.

### Approach Notes
1. Mapping scoped to class are not required for more generalized mappings such as those involving Dublin Core metadata or Schema.org terms. Classes are intentionally broad and therefore the context is not applicable. 
2. Whenever possible, mapping predicates should adhere to the SSSOM specification described here: https://mapping-commons.github.io/sssom/mapping-predicates/
3. Class mappings are assessed based on 1) Comparison of the class and object class definitions, 2) Alignment of class properties between the subject and object class.
4. Semantic mapping strategies that begin with class mappings require that classes in both the subject and object sources are defined.
5. The class mapping strategy is the recommended strategy for the following circumstances: 1) Vocabularies belonging to the same knowledge domain with a shared purpose/intent, 2) One of the standards is XSD-based (see note below)
6. In XSD-based standards, a single term may belong to multiple classes. Therefore, the term can be only be understood by the class it belongs to. 
The label property belongs to the 5 following classes: SampleRelation, MaterialSampleRecord, SamplingEvent, MaterialSampleCuration, and SamplingSIte. Label is globally defined as "A human intelligible string used to identify a thing, i.e. the name to use for the thing; should be unique in the scope of a sample collection or dataset.". Therefore, the parent class is required to understand how and where label is used and how label can be mapped to an object standard (Darwin Core).


Ben Norton
michaelnorton.ben@gmail.com


