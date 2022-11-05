# Pathology Markup Language (PathoML)



## Brief Introduction

A significant opportunity emerges to advance data-driven cancer research by performing integrative analysis on large-scale multimodal biomedical data using computational models. However, in addition to the mere amounts and number of modalities, the value of data for data-driven cancer research lies in biologically and medically meaningful features a large multimodal data contain. Although deep-learning techniques have enabled researchers to extract large-scale features from data, it remains time-consuming and error-prone for computational methods to access and use these features for diagnostic or scientific purposes, as a result of lacking a supporting data standard. Consequently, the potential of data to inform cancer research remains largely untapped. Here we propose Pathology mark-up language (i.e. PathoML) and Tumor Pathology Ontology to systematically represent heterogeneous features across multi-modal pathology data including pathology reports and digital slides in a form suitable for use by computational models. We pilot PathoML in representing pathological features contained in pathology data of several neoplastic diseases and exemplify different uses of the representations. The example representation files, the source code of the uses cases, Tumor Pathology Ontology, as well as the ontology specification and documentation of PathoML are available in this website.


## Links

PathoML [ontology specification](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Ontology%20Specification) and [documentation](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Documentation)

Representation Examples

- [Immunophenotypes](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Representation_Examples/Immunophenotypes)
- [Differentiated Subtyping Process of Lymphoma](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Representation_Examples/Differential%20Subtyping%20Process%20of%20Lymphoma)
- [Subtyping Process of Endocervical Carcinoma](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Representation_Examples/Process%20of%20Subtyping%20Endocervical%20Adenocarcinoma)

Use Cases

- [Automatic Diagnosis](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Use_Cases/Automatic%20Diagnosing)
- [HER2 Calculation](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Use_Cases/HER2%20Calculation)
- [Population-based Prognosis Analysis](https://github.com/Peiliang/pathoml.github.io/tree/main/Specification/Use_Cases/Population-based%20Prognosis%20Analysis)

[Tumor Pathology Ontology](https://github.com/Peiliang/pathoml.github.io/tree/main/Tumor%20Pathology%20Ontology)



## "Hello World" example

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" 
	xmlns:owl="http://www.w3.org/2002/07/owl#" 
	xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" 
	xmlns:histo="https://pathoml-1308125782.cos.ap-chengdu.myqcloud.com/PathoML.owl#"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema#">
	<owl:Ontology rdf:about="">
        	<owl:imports rdf:resource="https://pathoml-1308125782.cos.ap-chengdu.myqcloud.com/PathoML.owl"/>
	</owl:Ontology>
	<histo:NeoplasticCell rdf:ID="Hello_World_Cell">
		<histo:displayName rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Hello World</histo:displayName>
	</histo:NeoplasticCell>
</rdf:RDF>
```



## PathoML Team

[Chen Li's group](http://www.chenli.group/home)

