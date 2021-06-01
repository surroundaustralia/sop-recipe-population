# Population KG
This repository contains a _SOP Recipe_, that is a collection of mainly RDF assets, described by a _manifest_, used to create a multi-part Knowledge Graph (KG). This Knowledge Graph is usually used within the _SURROUND Ontology Platform_ (SOP) but can be loaded into other context-aware triplestores.

The IRI of the manifest - as a _register_ of assets, is:

* **<https://data.surroundaustralia.com/manifest/population/register>**


## Content
The main data within this KG are the data graphs within the `edg/datagraphs/` folder, however these are implemented in multiple files (dataset metadata in one, data in another), so the best way to see the data listing is within the manifest file, `edg/manifest.ttl`. There data graphs are indcated by assigning them the type <http://teamwork.topbraidlive.org/datagraph/datagraphprojects#ProjectType>, which is the TopQuadrant class for a data project item.

Supporting ontologies & SHACL shapes and taxonomies are stored within `edg/ontologies/` & `end/taxonomies/` folders respectively.

The ontologies and shapes are imported into a graph closure of the data graphs on load due to their 'including' within the manifest's listed suppliemnts for the data graphs.

### Queries
As these are developed, they will be added to the `queries/` folder.

## Provenance
The primary data for the data graphs in this repository is experimentally-released versions of the [Australian Bureau of Statistcs'](https://www.abs.gov.au/) census 2016 population change data. No changes have been made to this data here, only a format change from the provided XML to RDF.

The main ontolgies used to model this data are W3C standard ontologies, such as [SOSA](https://www.w3.org/TR/vocab-ssn/) and the [FSDF LINK](https://link.fsdf.org.au/) data mode in OWL form, the [FSDF Ontology](https://linked.data.gov.au/def/fsdf).

The data here was converted into RDF using custom Python scripts created for the [Loc-I DR Project](https://ldr.surroundaustralia.com) by [SURROUND Australia](https://surroundaustralia.com).

## License
For novel works in this repositry, the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) applies (see the [license deed](LICENSE)) however note that the source data for this work comes from elsewhere - see above.

## Contact
**Nicholas J. Car**  
*Data System Architect*  
SURROUND Australia Prt Ltd.  
<nicholas.car@surroundaustralia.com>  
<http://surroundaustralia.com>  