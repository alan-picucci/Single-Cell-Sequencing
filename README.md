# Single-Cell Sequencing Analysis

This repository contains a data analysis and machine learning project developed for the **Bocconi AI Lab (2022)**.  
The goal of the project is to analyze **single-cell RNA sequencing (scRNA-seq)** data and build models capable of distinguishing **hypoxic** and **normoxic** tumorous cells based on their gene expression profiles.

The project was awarded **first place** in the competition and was presented at the **Department of Oncology of Oxford University**, within the *Bioinformatics Hub conference series*.

---

## Project Overview

Single-cell RNA sequencing produces high-dimensional, sparse, and noisy data, requiring careful preprocessing and analysis before reliable modeling can be performed.  
In this project, we developed a complete pipeline that includes:

- Exploratory analysis of gene expression data
- Data filtering and normalization at both cell and gene level
- Dimensionality reduction for visualization and feature extraction
- Unsupervised learning to uncover structure in the data
- Supervised learning to classify hypoxic vs normoxic cells

The analysis is entirely documented in the accompanying Jupyter Notebook.

---

## Data

The dataset consists of single-cell RNA sequencing data from two cancer cell lines:

- **HCC1806**
- **MCF7**

Data were generated using different sequencing technologies (e.g. Smart-Seq and Drop-Seq), resulting in varying sparsity and noise characteristics.  
Each observation corresponds to a single cell, represented by a high-dimensional vector of gene expression values.

---

## Exploratory Data Analysis

We begin by exploring the statistical properties of the data to assess quality and identify potential sources of noise.  
This includes:

- Distribution of gene expression counts
- Sparsity patterns across cells
- Identification of low-quality or misrecorded cells
- Analysis of gene variability across the population

Based on these insights, we apply filtering criteria to remove uninformative cells and genes, improving downstream analysis.

---

## Unsupervised Analysis

To better understand the structure of the data and reduce dimensionality, we apply several unsupervised techniques, including:

- Dimensionality reduction methods for visualization and representation learning
- Clustering algorithms to identify groups of cells with similar expression profiles

These methods help reveal latent structure in the data and guide feature selection for supervised learning.

---

## Supervised Learning

In the final stage, we train machine learning models to classify cells as hypoxic or normoxic.  
Key aspects of this phase include:

- Feature engineering informed by preprocessing and unsupervised analysis
- Evaluation of multiple classification models
- Cross-validation for model selection
- Assessment of generalization performance on held-out data

The combination of preprocessing, representation learning, and model selection leads to strong classification performance across cell lines and sequencing techniques.

---

## Repository Structure

- `Group_3_Final_Report.ipynb` — Complete analysis, including methodology, experiments, and results
- `License` - BSD 3-Clause License
- `README.md` — Project overview and description

---

## Authors

This project was developed by **Group 3** as part of the Bocconi AI Lab:

- Dario Filatrella  
- Rocco Giampetruzzi  
- Rolf Minardi
- **Alan Picucci**  
- Mattia Scardecchia
- Klejdi Sevdari  

---

