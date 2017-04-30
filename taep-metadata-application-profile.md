Contributing Institution: Rutgers University

Mandatory Elements: The following 7 elements have been adapted from Dublin Core and the Text Encoding Initiative (TEI) for the purposes of describing metadata for Correspondences within the larger Thomas A. Edison Papers (TAEP).  In order to ensure consistency and interoperability with TAEP's existing database, the following elements are mandatory for every correspondence record:
Title
Identifier
Subject
Publisher
Source
Date
Correspondence Description
Relation

The following refinements to 'Relation' are mandatory in all correspondence records:
Is Part Of
Has Part

Title:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.title
Label: Title
Dublin Core Definition: The name given to the resource
Dublin Core Comment: Typically, the Title will be a name by which the resource is formally known.
TAEP Comment: Every title in the TAEP Correspondence Collection follows a format of "letter from x to y".
TAEP Derived Element(s): name, name_code
TAEP Derived Table(s): names, names_in_documents
Mandatory: Yes
Repeatable: No
Qualifiers: None


Identifier:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.identifier
Label: Document_id, Reel/Frame
Dublin Core Definition: An unambiguous reference to the resource within a given context.
Dublin Core Comment: Recommended best practice is to identify the resource by means of a string conforming to a formal identification system.
TAEP Comment: This field will appear twice in most - if not all - correspondence records in TAEP.  This is necessary, because every correspondence record has both a unique ID number, as well as existing in microfilm.
TAEP Derived Element(s): document_id, reel, frame
TAEP Derived Table(s): document_records
Mandatory: Yes
Repeatable: Yes
Qualifiers: None


Subject:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.subject
Label: Description, Name Mentions
Dublin Core Definition: The topic of the resource.
Dublin Core Comment: Typically, the subject will be represented using keywords, key phrases, or classification codes. Recommended best practice is to use a controlled vocabulary.
TAEP Comment: This field will appear once in each record, although it contains multiple fields from the TAEP database.  This field will combine a description of the document subject matter with a list of relevant names mentioned in the document.
TAEP Derived Element(s): description, name_code, name
TAEP Derived Table(s): names, names_in_documents, subjects
Mandatory: Yes
Repeatable: No
Qualifiers: None


Publisher:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.publisher
Label: Publisher
Dublin Core Definition: An entity responsible for making the resource available.
Dublin Core Comment: Examples of a Publisher include a person, an organization, or a service. Typically, the name of a Publisher should be used to indicate the entity.
TAEP Comment: Every correspondence record in the collection will contain a reference to 'The Thomas Edison Papers, part of The School of Arts and Sciences, Rutgers, The State University of New Jersey'
TAEP Derived Element(s): n/a
TAEP Derived Table(s): n/a
Mandatory: Yes
Repeatable: No
Qualifiers: None


Source:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.source
Label: Source
Dublin Core Definition: A related resource from which the described resource is derived.
Dublin Core Comment: The described resource may be derived from the related resource in whole or in part. Recommended best practice is to identify the related resource by means of a string conforming to a formal identification system.
TAEP Comment: This field is a reference to the physical repository in which the original archival document - upon which the digital document is based - is contained.
TAEP Derived Element(s): credit_line
TAEP Derived Table(s): locations
Mandatory: Yes
Repeatable: No
Qualifiers: None


Date:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.date
Label: Date
Dublin Core Definition: A point or period of time associated with an event in the lifecycle of the resource.
Dublin Core Comment: Date may be used to express temporal information at any level of granularity. Recommended best practice is to use an encoding scheme, such as the W3CDTF profile of ISO 8601 [W3CDTF].
TAEP Comment: This field is a reference to the date associated with the original document and the relevant digital file it is derived from.
TAEP Derived Element(s): doc_date
TAEP Derived Table(s): document_records
Mandatory: Yes
Repeatable: No
Qualifiers: None


Correspondence Description:

Namespace: http://www.tei-c.org/ns/1.0
Root Element: <teiHeader> -> <profileDesc> -> <correspDesc>
Label: Correspondence Description
Secondary element(s): <correspAction>
Tertiary element(s): <persName>, <orgName>, <date>, <settlement>
TEI Definition: <correspDesc> (correspondence description) contains a description of the actions related to one act of correspondence.
TEI Comment: The correspDesc element is used within the profileDesc element to provide detailed correspondence-specific metadata, concerning in particular the communicative aspects (sending, receiving, forwarding etc.) associated with an act of correspondence. This information is complementary to the detailed descriptions of physical objects (such as letters) associated with correspondence acts, which are typically provided by the sourceDesc element.
TAEP Comment: The TEI namespace provides the most detailed metadata schema for correspondence descriptions amongst the various schemas that we explored for this project.
TAEP Derived Element(s): name, doc_date
TAEP Derived Table(s): names, names_in_documents, document_records
Mandatory: Yes
Repeatable: No
Qualifiers: None


Is Part Of:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.relation.isPartOf
Label: Is Part Of
Dublin Core Definition: A related resource in which the described resource is physically or logically included.
Dublin Core Comment: This term is intended to be used with non-literal values as defined in the DCMI Abstract Model (http://dublincore.org/documents/abstract-model/). As of December 2007, the DCMI Usage Board is seeking a way to express this intention with a formal range declaration.
TAEP Comment: This term will be used to relate the digital file - itself a conceptual representation of a combination of physical pages - to the larger series to which it is a part of within the collection.
TAEP Derived Element(s): gloc
TAEP Derived Table(s): document_records
Mandatory: Yes
Repeatable: No
Qualifiers: None


Has Part:

Namespace: http://dublincore.org/documents/dcmi-terms/
Root Element: dc.relation.hasPart
Label: Has Part
Dublin Core Definition: A related resource that is included either physically or logically in the described resource.
Dublin Core Comment: This term is intended to be used with non-literal values as defined in the DCMI Abstract Model (http://dublincore.org/documents/abstract-model/). As of December 2007, the DCMI Usage Board is seeking a way to express this intention with a formal range declaration.
TAEP Comment: This term will provide a link to the actual images associated with the physical document of which the digital file is a representation.
TAEP Derived Element(s): image_id
TAEP Derived Table(s): images
Mandatory: Yes
Repeatable: No
Qualifiers: None
