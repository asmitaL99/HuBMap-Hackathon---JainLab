# HuBMap-Hackathon--- Imaging Based Spatial Transcriptomics Pipeline

# Overview
This repository provides an end-to-end pipeline for the analysis of imaging-based spatial transcriptomics (ST) datasets, focusing on quality control (QC), cell type annotation, and neighborhood analysis. The pipeline was developed as part of the HuBMAP project and is designed to process datasets from different imaging technologies, including Xenium, MERFISH, and CosMx, across multiple tissue types such as kidney, intestine, and lung.

Imaging-based spatial transcriptomics technologies are underexplored within the HuBMAP community, and this pipeline aims to fill that gap by providing tools specifically designed for the analysis of such data.

# Features
Quality Control: Comprehensive QC metrics for imaging-based ST datasets.
Cell Type Annotation: Leverages reference single-cell RNA-seq data for accurate cell type labeling.
Neighborhood Analysis: Performs spatial neighborhood analysis using multiple software packages to compare results across tissues.
Cross-Tissue Comparison: Supports multi-tissue datasets for comparative analysis (e.g., kidney, lung, intestine).

# Tools & Packages
The pipeline leverages the following tools:

### Squidpy: For spatial analysis of single-cell and spatial transcriptomics data.
### Scanpy: For single-cell RNA-seq data processing and analysis.
### Scipy: For statistical and mathematical operations.
### TACCO: For cell type annotation based on reference single-cell datasets.
### Monkeybread: A tool for spatial neighborhood analysis.

# Inputs
## Cell Metadata:
cells.csv: Contains cell-level metadata such as cell ID, coordinates, and more.
## Gene Expression Matrix:
cell_feature_matrix.h5: A cell-by-gene matrix read into an AnnData object.
## Reference Annotations:
Single-cell RNA-seq reference annotation data in AnnData format.

