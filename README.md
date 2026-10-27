# integMET-rdf

RDF data and schema files for integMET, integrating metabolomics study metadata from MetaboLights and Metabolomics Workbench.

## Data model

The data connects studies, assays, sample groups, within-assay comparisons, and annotated compounds:

- **Study**: source identifiers, study summaries, organism information, and biological annotations such as GO, MeSH, NCBI Gene, and OMIM links.
- **Assay**: analytical methods, source file names, sample counts, and links to sample groups, comparisons, and compounds.
- **SampleGroup**: sample identifiers and group metadata, including species, tissue, and control-group information.
- **DiffProf**: a comparison between a reference group and a condition group, with descriptions of the contrast and its biological relevance.
- **AnnotatedCompound**: a molecular entity identified by an InChIKey.

The local vocabulary uses `http://integmet.org/ontology/` alongside standard RDF vocabularies and external identifiers.

## Files

| File | Description |
| --- | --- |
| [integmet_v1.ttl](integmet_v1.ttl) | RDF data in Turtle format, suitable for reading and inspection. |
| [integmet_v1.nt](integmet_v1.nt) | RDF data in N-Triples format, with one triple per line. |
| [integmet_v1.jsonld](integmet_v1.jsonld) | RDF data in JSON-LD format. |
| [integmet_integrated_rdf.linkm_20261007.yaml](integmet_integrated_rdf.linkm_20261007.yaml) | LinkML schema defining classes, properties, and constraints. |
| [integMET/model.yaml](integMET/model.yaml) | RDF-config model describing resource relationships with example values. |
| [integMET/prefix.yaml](integMET/prefix.yaml) | Namespace prefixes used by the RDF-config model. |
| [integMET/endpoint.yaml](integMET/endpoint.yaml) | Local SPARQL endpoint configuration. |
| [integMET/integMET.svg](integMET/integMET.svg) | RDF model diagram. |
| [integMET/memo.txt](integMET/memo.txt) | Command note for generating the diagram with RDF-config. |
