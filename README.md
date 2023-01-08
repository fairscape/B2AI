# README


This repository contains metadata dictionaries, class models and their instances of
computations, datasets, and software described in the Multi-Scale Integrated Cell
(MuSIC) pipeline which integrates protein fluorescent images and protein
biophysical association data to create a unified hierarchical map of human cell
architecture. A detailed provenance map [here](./CM4AI/CM4AI%20Data%20Dictionary%20-%20MuSIC%201.0%20Provenance%20Model.png) shows each component required to run the pipeline. In our current release, only the components within the rectangle titled `Ideker Lab/MuSIC` have been addressed by the data dictionary, metadata model and instances.   

More information on the MuSIC pipeline:

* [Publication](https://www.biorxiv.org/cgi/content/short/2020.06.21.163709v1)
* [Github](https://github.com/idekerlab/MuSIC)
* [Step-by-step Guide](https://github.com/idekerlab/MuSIC/wiki/A-Step-By-Step-Guide-to-Building-a-MuSIC-Map)

The models and instances are expressed using the Linked Data Modeling Language
framework called LinkML.

For more information on LinkML:

* [linkml.io](https://linkml.io) main website
* [specification](https://linkml.io/linkml-model/docs/specification/)


## Data dictionary
Directory `data-dictionary` contains three data dictionary documents which are still at their infancy.

* [computation.md](./CM4AI/data-dictionary/computation.md)
* [dataset.md](./CM4AI/data-dictionary/dataset.md)
* [software.md](./CM4AI/data-dictionary/software.md)

The current release contains metadata about objects using a select set of variables, their data types, preferred mapping using URIs/CURIEs, and allowed values based on the current state of the MuSIC pipeline. More detailed version of the data dictionary is planned for release in future. For example, the dictionary for Dataset (`dataset.md`) introduces a slot (aka attribute/property) called `schema` which refers to the schema of the content. As different formats of the content demand different schema representation, more work in this direction is required.

## Models
Directory `linkml-models` contains three LinkML models for Dataset, Software, and Computation. The models are currently represented as flat structure. In future release, nested structure will be used with support from the advanced features in the LinkML [ecosystem](https://linkml.io/linkml/ecosystem.html).   

* LinkMLMuSICComputationModel
* LinkMLMuSICDatasetModel
* LinkMLMuSICSoftwareModel

## Instances


There are many subsets of *profiles* of the metamodel, for different purposes:
The instances of Computation, Dataset and Software described in the following directories can be [validated](https://linkml.io/linkml/intro/tutorial02.html#validating) against the metadata model:

* linkml-computation-instances
* linkml-dataset-instances
* linkml-software-instances
