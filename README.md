# mRNA-seq-differential-expression-analysis-using-R-with-pathway-enrichment-

# CLL_cancerVSnormal
#
# Overview:
# This script performs differential gene expression analysis on Chronic Lymphocytic Leukemia (CLL) data,
# comparing cancer and normal samples using DESeq2.
#
# Requirements:
# - R (version 4.0 or higher recommended)
# - Packages: msigdbdf, msigdbr, DESeq2, tidyverse
#
# Installation:
# The script installs required packages if not already installed:
# if (!requireNamespace("BiocManager", quietly = TRUE))
#   install.packages("BiocManager")
# BiocManager::install(c("msigdbdf", "msigdbr", "DESeq2"))
# install.packages("tidyverse")
#
# Input Data:
# - counts.csv: Raw count matrix of gene expression data (genes x samples)
# - CLL_meta.csv: Metadata containing sample information and condition labels (cancer or normal)
# Ensure sample names in both files match for correct analysis.
#
# Script Workflow:
# 1. Load libraries and data.
# 2. Match samples between count data and metadata.
# 3. Create DESeq2 dataset and run differential expression analysis.
# 4. Extract results including gene names, log fold changes, and p-values.
#
# Output:
# A data frame containing differential expression results for all genes, ready for downstream analysis.
#
# Usage:
# Run the script in an R environment after setting your working directory to the folder containing your input files.


