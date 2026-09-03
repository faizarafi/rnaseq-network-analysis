# RNA-seq Differential Expression Analysis & Network Analysis (Anonymized Project)

## Overview

An end-to-end RNA-seq analysis workflow integrating differential expression, functional enrichment, and gene regulatory network analysis.

This repository contains an anonymized version of an RNA-seq project developed for an unpublished research dataset. The analysis demonstrates transcriptomic data processing, differential expression analysis, downstream functional interpretation, and network-based analysis of gene regulation.

**Note:** Because the original dataset is unpublished, sample metadata, gene identifiers, raw sequencing data, and project-specific results have been removed or anonymized.

## Analysis Workflow

RNA-seq data → expression quantification → normalization → differential expression → functional enrichment → regulatory/network analysis

1. Expression Data Processing
- Processed RNA-seq expression data generated from an upstream alignment/quantification workflow
- Imported transcript-level abundance estimates using tximport
- Prepared count matrices for downstream analysis
  
2. Differential Expression Analysis

Differential expression analysis was performed using DESeq2, including:
- Count normalization
- Experimental group comparisons
- Principal component analysis (PCA)
- Differentially expressed gene identification
- Volcano plots
- Heatmaps
- Venn and UpSet plots for comparison of gene sets
  
3. Functional Interpretation

Differentially expressed genes were evaluated using functional enrichment analysis, including:
- Gene Ontology (GO) enrichment
- Functional category analysis
- Comparison of enriched gene sets across experimental conditions

4. Regulatory Network Analysis
   
The project extended beyond differential expression to investigate potential gene regulatory relationships using:
- WGCNA for co-expression network analysis
- GENIE3 for gene regulatory network inference
- Integration of regulatory information from DAP-seq data

These analyses were used to identify groups of co-expressed genes and investigate potential regulatory relationships underlying transcriptional differences.

## Tools and Technologies
| Category | Tools |
|---|---|
| RNA-seq processing | `RSEM`, `STAR`, `tximport` | 
| Differential expression | `DESeq2` | 
| Network analysis | `WGCNA`, `GENIE3` | 
| Functional analysis | `Gene Ontology enrichment` |
| Visualization | `ggplot2`, `heatmaps`, `PCA`, `volcano plots`, `upset plots`|
| Languages | `R`, `Python`, `Bash`|
| Environment | `Linux/HPC`|

## Technical Skills Demonstrated
- RNA-seq data analysis
- Count-matrix processing and normalization
- Differential expression analysis
- Multivariate transcriptomic analysis
- Functional enrichment
- Gene co-expression network analysis
- Gene regulatory network inference
- Integration of transcriptomic and regulatory datasets
- Reproducible analysis using R/Python/Bash

## Contents
`dge_network_proj_workflow.ipynb`: Step-by-step notebook for processing a counts matrix, performing normalization and differential expression with DESeq2, and generating basic plots (e.g., PCA, venn, volcano, heatmap, upset plots). Function annotation analysis with Gene ontology terms is also conducted. Part II involved gene regulatory network analysis with dap-seq data and WCGNA.

## Data Availability & Anonymization

The original dataset was generated as part of an unpublished research project and is not included in this repository.

To protect unpublished research and associated metadata:

Raw sequencing data are not included
Sample metadata have been anonymized
Gene identifiers have been removed or anonymized
Project-specific results and figures have been removed

The repository therefore demonstrates the analysis workflow and computational methods rather than providing a fully reproducible analysis of the original dataset.

Notes:
This repository is intended as a portfolio example of transcriptomic and network-analysis workflows applied to biological research data. The available notebook has been modified to remove information associated with the unpublished dataset.

