

# For evolutive (version independent work)

```sparql
PREFIX cdm: <http://publications.europa.eu/ontology/cdm#>
PREFIX lg: <http://publications.europa.eu/resource/authority/language/>
PREFIX lbl: <http://publications.europa.eu/resource/authority/label-type/>
PREFIX org: <http://www.w3.org/ns/org#>
PREFIX owl:<http://www.w3.org/2002/07/owl#>
PREFIX ev: <http://eurovoc.europa.eu/>
PREFIX euvoc: <http://publications.europa.eu/ontology/euvoc#>
PREFIX skos:<http://www.w3.org/2004/02/skos/core#>
prefix dstype: <http://publications.europa.eu/resource/authority/dataset-type/>
SELECT DISTINCT *
WHERE {
    values (?workPublicId ) { (<http://publications.europa.eu/resource/dataset/corporate-body> ) }
    ?workCellarId owl:sameAs ?workPublicId . 
    ?expressionCellarId cdm:expression_belongs_to_work ?workCellarId .
    ?expressionCellarId owl:sameAs ?expressionPublicId .
    ?manifestationCellarId cdm:manifestation_manifests_expression ?expressionCellarId .
    ?manifestationCellarId owl:sameAs ?manifestationPublicId .
    ?itemCellarId cdm:item_belongs_to_manifestation ?manifestationCellarId .
    ?itemCellarId owl:sameAs ?itemPublicId .
}
```
 




# ?workCellarId properties

http://www.w3.org/2002/07/owl#sameAs
http://www.w3.org/1999/02/22-rdf-syntax-ns#type
http://publications.europa.eu/ontology/cdm#work_title
http://publications.europa.eu/ontology/cdm#work_published_in_work
http://publications.europa.eu/ontology/cdm#work_id_document
http://publications.europa.eu/ontology/cdm#work_id
http://publications.europa.eu/ontology/cdm#work_date_document
http://publications.europa.eu/ontology/cdm#work_date_creation
http://publications.europa.eu/ontology/cdm#work_dataset_version
http://publications.europa.eu/ontology/cdm#work_dataset_published_by_agent
http://publications.europa.eu/ontology/cdm#work_dataset_keyword
http://publications.europa.eu/ontology/cdm#work_dataset_has_type_concept_type_dataset
http://publications.europa.eu/ontology/cdm#work_dataset_has_frequency_publication_frequency
http://publications.europa.eu/ontology/cdm#work_dataset_has_documentation_documentation
http://publications.europa.eu/ontology/cdm#work_dataset_description_editorial
http://publications.europa.eu/ontology/cdm#work_dataset_date_start
http://publications.europa.eu/ontology/cdm#work_dataset_date_modified
http://publications.europa.eu/ontology/cdm#work_created_by_agent
http://publications.europa.eu/ontology/cdm#do_not_index
http://publications.europa.eu/ontology/cdm#datetime_transmission
http://publications.europa.eu/ontology/cdm#datetime_negotiation
http://publications.europa.eu/ontology/cdm/cmr#lastModificationDate
http://publications.europa.eu/ontology/cdm/cmr#creationDate

 
# ?workPublicId properties 

None

# ?expressionCellarId properties

http://www.w3.org/2002/07/owl#sameAs
http://www.w3.org/1999/02/22-rdf-syntax-ns#type
http://publications.europa.eu/ontology/cdm#expression_uses_language
http://publications.europa.eu/ontology/cdm#expression_title
http://publications.europa.eu/ontology/cdm#expression_belongs_to_work
http://publications.europa.eu/ontology/cdm/cmr#lastModificationDate
http://publications.europa.eu/ontology/cdm/cmr#lang
http://publications.europa.eu/ontology/cdm/cmr#creationDate

# ?expressionPublicId properties 

None

# ?manifestationCellarId properties
http://www.w3.org/2002/07/owl#sameAs
http://www.w3.org/1999/02/22-rdf-syntax-ns#type
http://publications.europa.eu/ontology/cdm#manifestation_type
http://publications.europa.eu/ontology/cdm#manifestation_manifests_expression
http://publications.europa.eu/ontology/cdm#manifestation_distribution_has_status_distribution_status
http://publications.europa.eu/ontology/cdm#manifestation_distribution_has_media_type_concept_media_type
http://publications.europa.eu/ontology/cdm#manifestation_distribution_date_modified
http://publications.europa.eu/ontology/cdm#manifestation_date_publication
http://publications.europa.eu/ontology/cdm/cmr#lastModificationDate
http://publications.europa.eu/ontology/cdm/cmr#creationDate

# ?manifestationPublicId properties

None

# ?itemCellarId properties

http://www.w3.org/2002/07/owl#sameAs
http://www.w3.org/1999/02/22-rdf-syntax-ns#type
http://publications.europa.eu/ontology/cdm#item_identifier
http://publications.europa.eu/ontology/cdm#item_belongs_to_manifestation
http://publications.europa.eu/ontology/cdm/cmr#manifestationMimeType

# ?itemPublicId properties

None

