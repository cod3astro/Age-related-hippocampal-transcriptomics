# Transcriptomic Insights Into Age-Related Hippocampal Changes in Rats

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX) <!-- Replace with actual DOI if you archive there -->
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Overview
This repository contains the complete computational workflow and data for the study **"Transcriptomic Insights into Age-Related Hippocampal Changes in Rats"**. The project re-analyses a public microarray dataset (GDS3915) to characterize age-dependent gene expression changes in the rat hippocampus across five time points (3, 6, 9, 12, and 23 months). We identify a late-life neuroinflammatory signature involving complement activation, lysosomal pathways, and immune dysregulation.

The analysis is performed in Python and includes differential expression testing, functional enrichment (GO/KEGG), and visualisation (PCA, volcano plots, heatmaps).

## Authors
- **Tijani Abdullateef Pelumi**  
  University of Ilorin  
  📧 molabosipolateef@gmail.com  

## Data Source
The raw gene expression data were obtained from the **NCBI Gene Expression Omnibus (GEO)** under accession [GDS3915](https://www.ncbi.nlm.nih.gov/sites/GDSbrowser?acc=GDS3915).  
Original experiment: *Kadish, I. et al. (2007). Transcriptional profiles of rodent hippocampal CA1 tissue during aging and cognitive decline.*  
- Platform: Affymetrix Rat Expression 230A Array [GPL341]  
- Samples: 49 male Fischer 344 rats (3, 6, 9, 12, 23 months)

## Repository Contents
- `GDS3915.ipynb` – Jupyter notebook containing the full analysis pipeline (data loading, preprocessing, statistics, visualisation).
- `GDS3915.soft` – The original SOFT format file downloaded from GEO (optional – you may also provide a download script to save space).
- `requirements.txt` – List of Python dependencies required to run the notebook.
- `README.md` – This file.
- `LICENSE` – MIT license (or choose another).

## Requirements
The analysis was performed with Python 3.13 and the following key libraries:
- `GEOparse` – for parsing the SOFT file
- `pandas`, `numpy` – data manipulation
- `scikit-learn` – PCA, scaling
- `matplotlib`, `seaborn` – visualisation
- `scipy` – statistical tests
- `gseapy` – gene set enrichment analysis
- `statsmodels` – multiple testing correction

Install all dependencies using:
```bash
pip install -r requirements.txt
