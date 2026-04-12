# Parkinson Protein Classification Dataset

## Description
This repository contains protein sequences associated with Parkinson’s disease and control proteins, curated for binary classification tasks in bioinformatics and machine learning.

The dataset is structured as a binary classification problem with two classes:
- Parkinson-associated proteins (label = 1)
- Control proteins (label = 0)

## Dataset Versions

### Original version (v1.0)
- Total samples: 306 proteins
- Parkinson-associated proteins: 153
- Control proteins: 153

### Cleaned version (v2.0)
- Total samples: 304 proteins
- Removed duplicated sequence appearing in both classes (data leakage)
- Identified one sequence containing a non-standard amino acid (U, selenocysteine), which is retained in this version

The cleaned dataset is provided as:

`parkinson_dataset_v2.csv`

## Data Format
Each record in the dataset includes the following fields:
- `id`: protein identifier (UniProt accession and name)
- `descripcion`: protein description from UniProt
- `secuencia`: amino acid sequence
- `longitud`: sequence length (number of amino acids)
- `label`: class label (1 = Parkinson-associated, 0 = control)

## Data Source
Protein sequences were obtained from the UniProt database and curated for classification purposes.

## Official Dataset (Zenodo)
The authoritative and citable version of this dataset is available in Zenodo:

https://doi.org/10.5281/zenodo.19544048

Version 2.0 of the dataset was used in the experiments.

## License
This dataset is distributed under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

You are free to share and adapt the material, provided appropriate credit is given to the original author.

## Reproducibility
Both the original and cleaned versions are provided to ensure reproducibility and transparency in experimental evaluation.
