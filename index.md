# Pathology Markup Language (PathoML)



## Brief Introduction

Computational pathology provides "big-data" approach to pathology, having substantial implications for cancer research and medicine. However, the large-scale implementation of computational pathology has been hindered by the lack of a standardized format representing various histopathological features in histopathology data. Here we propose Histopathology Markup Language (HistoML) and Histopathology Ontology for precisely representing various histopathological features in tumor, observed from whole-slide-images, at different granularity and in a machine-understandable format. We pilot HistoML in representing histopathological features contained in histopathology data of several neoplastic diseases and exemplify different uses of the representations. The example representation files, the source code of the uses cases, Histopathology Ontology, as well as the ontology specification and documentation of HistoML Level1 are available in this website.


## Links

HistoML [ontology specification](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Ontology_Specification) and [documentation](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Documentation)

Representation Examples

- [Rhabdoid Cells](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Representation_Examples/Rhabdoid_cells)
- [Alveolar Pattern](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Representation_Examples/Alveolar_pattern)
- [Tumors Extending into Renal Sinus](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Representation_Examples/Tumors_extending_into_renal_sinus)
- [Papillary thyroid cancer](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Representation_Examples/Papillary%20thyroid%20cancer)

Use Cases

- [Tumor-Immune Phenotype Characterization](https://github.com/Peiliang/HistoML/tree/master/Specification/Level1/Use_Cases/Tumor-Immune%20Phenotype%20Characterization)

[Histpathology Ontology](https://github.com/Peiliang/HistoML/tree/master/Histopathology%20Ontology)



## "Hello World" example

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" 
	xmlns:owl="http://www.w3.org/2002/07/owl#" 
	xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" 
	xmlns:histo="http://www.semanticweb.org/release/HistoML1.owl#"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema#">
	<owl:Ontology rdf:about="">
        	<owl:imports rdf:resource="http://www.semanticweb.org/release/HistoML1.owl"/>
	</owl:Ontology>
	<histo:NeoplasticCell rdf:ID="Hello_World_Cell">
		<histo:displayName rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Hello World</histo:displayName>
	</histo:NeoplasticCell>
</rdf:RDF>
```



## HistoML Team

[Chen Li's group](http://www.chenli.group/home)

