## Terminology 

| Term             | Definition | URI | Remarks          |
| -- | -- | -- | -- |
| Broader          | A related term that is more general in meaning. Also establishes a hierarchical link where the related term is the immediate parent concept.  |    |   |
| broadMatch       | A mapping relation where the object is a broader concept than the subject.| http://www.w3.org/2004/02/skos/core#broadMatch          |   |
| Class            | Description of a set of objects that share the same attributes, operations, methods, relationships, and semantics              | ISO 11179             |   |
| ClassDefinition  | An element whose instances are complex objects that may have slot-value assignments_         | LinkML Metamodel      |   |
| closeMatch       | A mapping relation where the subject and object are sufficiently similar that they can be used interchangeably in some information retrieval applications.       | [https://www.w3.org/2009/08/skos-reference/skos.html#closeMatch](https://www.w3.org/2009/08/skos-reference/skos.html#closeMatch)           |   |
| Concept          | The units of thought which underlie many knowledge organization systems.  | [http://www.w3.org/2004/02/skos/core#Concept](http://www.w3.org/2004/02/skos/core#Concept)|   |
| Concept          | The units of thought which underlie many knowledge organization systems.  | [http://www.w3.org/2004/02/skos/core#Concept](http://www.w3.org/2004/02/skos/core#Concept)| Concepts exist in the mind as abstract entities which are independent of the terms used to label them.  |
| exactMatch       | A mapping relation where the subject and object are sufficiently similar, with a high degree of confidence, that they can be used interchangeably across a wide range of information retrieval applications.      | [https://www.w3.org/2009/08/skos-reference/skos.html#exactMatch](https://www.w3.org/2009/08/skos-reference/skos.html#exactMatch)           |   |
| Instance         | Named value belonging to a concept scheme   |    |   |
| Instance-based Matching Process | A matching process based on individual representations (or instances).    | https://w3id.org/semapv/vocab/InstanceBasedMatching     |   |
| Manual Mapping Curation         | An matching process that is performed by a human agent and is based on human judgement and domain knowledge.| https://w3id.org/semapv/vocab/ManualMappingCuration     | A human curator determines that a subject should be mapped to an object by virtue of their domain expertise.           |
| Mapping          | A triple comprising a subject entity s, an object entity o and a mapping predicate p.        | https://w3id.org/semapv/vocab/Mapping| The subject entity NCI:C9305 is mapped to the object entity ICD10:C80.9 using the skos:relatedMatch mapping predicate. |
| Mapping Relation | A mapping (alignment) between SKOS concepts in different concept schemes, where the links are inherent in the meaning of the linked concepts  | [https://www.w3.org/2009/08/skos-reference/skos.html#mappingRelation](https://www.w3.org/2009/08/skos-reference/skos.html#mappingRelation) |   |
| narrowMatch      | A mapping relation where the object is a narrower concept that the subject.   | [https://www.w3.org/2009/08/skos-reference/skos.html#narrowMatch](https://www.w3.org/2009/08/skos-reference/skos.html#narrowMatch)  |   |
| Normalization    | A family of preprocessing techniques for reducing strings to be compared to a common format. | https://w3id.org/semapv/vocab/Normalization             |   |
| Object           | Concept the subject is being mapped to  | SSSOM Specification   |   |
| Predicate        | A mapping annotation that is used to describe the mapping between the subject and object     |    |   |
| Property         | A quality common to all members of an object class         | ISO 11179             |   |
| Range            | Defines the type of the object of the slot. | LinkML Metamodel      |   |
| Related          | A related term (object) in an associative semantic relationship with the subject term, where the two concepts are not related hierarchically, but sufficiently similar to establish a functional relationship for information retrieval activities. |    |   |
| relatedMatch     | A mapping relation where the subject and the object are inherently related, but where none is in any way more general than the other.         | [https://www.w3.org/2009/08/skos-reference/skos.html#relatedMatch](https://www.w3.org/2009/08/skos-reference/skos.html#relatedMatch)       |   |
| Slot             | A top-level concept in the LinkML schema, slots are analogous to attributes, fields, columns, and properties can be associated with classes to specify what fields instances of that class can have| LinkML Metamodel      |   |
| SlotDefinition   | An element that describes how instances are related to other instances    | LinkML Metamodel      |   |
| Subject          | Concept being mapped     | SSSOM Specification   |   |
| TypeDefinition   | An element that whose instances are atomic scalar values that can be mapped to primitive types              | LinkML Metamodel      |   |


**See Resources for source information
