# SARS-CoV-2 Infection Dynamics – scRNA-seq Trajectory Analysis

## Project Overview
This project reproduces neighborhood clustering, cell state identification,
and pseudotime analysis of SARS-CoV-2–infected human bronchial epithelial cells,
based on the study:
PLOS Biology (2021): https://doi.org/10.1371/journal.pbio.3001143

## Dataset
- GEO Accession: GSE166766
- Data type: Single-cell RNA sequencing (scRNA-seq)
- Cells: Human bronchial epithelial cells
- Infection conditions: Mock, 1 dpi, 3 dpi

Processed count matrices provided by GEO were used to ensure reproducibility.

## Objectives
- Perform neighborhood clustering of epithelial cells
- Identify infection-associated cell states
- Reconstruct transcriptional trajectories using pseudotime
- Evaluate ACE2 and ENO2 as biomarkers of SARS-CoV-2 infection

## Methods Summary
- Quality control filtering
- Normalization and log transformation
- Highly variable gene selection
- PCA, neighborhood graph construction, Leiden clustering
- UMAP visualization
- Pseudotime inference (Scanpy-based)

## Key Notes and Limitations
- Clusters represent transcriptional states, not strict cell types
- Pseudotime reflects inferred progression, not real time
- ACE2 expression is sparse due to scRNA-seq dropout
- ENO2 provides a more robust infection-associated signal

## Files
- `analysis.ipynb`: Main analysis notebook
- `README.md`: Project overview and guidance

## Environment
- Python
- Scanpy
- NumPy, Pandas, Matplotlib

## Author
Kofoworola Aminat Salami
