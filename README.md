# Developing-an-infection-state-predictive-model

This repository contains code supporting the study from https://www.medrxiv.org/content/10.1101/2020.07.28.20163329v2. Scripts and functionality included are (1) multiple-step batch correction, (2) gene feature selection with backwards elimination implemented in VarSelRF with Ranger, (3) gene feature selection with a genetically inspired search algorithm, implemented with GALGO. 

## Abstract

A fundamental problem for disease treatment is that while antibiotics are a powerful counter to bacteria, they are ineffective against viruses. Often, bacterial and viral infections are confused due to their similar symptoms and lack of rapid diagnostics. With many clinicians relying primarily on symptoms for diagnosis, overuse and misuse of modern antibiotics are rife, contributing to the growing pool of antibiotic resistance. To ensure a given individual receives optimal treatment given their disease state and to reduce over-prescription of antibiotics, the host response can be measured quickly to distinguish between the two states. To establish a predictive biomarker panel of disease state (viral/bacterial/no-infection) we conducted a meta-analysis of human blood infection studies using Machine Learning (ML). We focused on publicly available gene expression data from two widely used platforms, Affymetrix and Illumina microarrays as they represented a significant proportion of the available data. We were able to develop multi-class models with high accuracies with our best model predicting 93% of bacterial and 89% viral samples correctly. To compare the selected features in each of the different technologies, we reverse engineered the underlying molecular regulatory network and explored the neighbourhood of the selected features. This highlighted that although on the gene-level the models differed, they did contain genes from the same areas of the network. Specifically, this convergence was to pathways including the Type I interferon Signalling Pathway, Chemotaxis, Apoptotic Processes, and Inflammatory / Innate Response. 

If used please cite: Myall, A.C., Perkins, S., Rushton, D., Jonathan, D., Spencer, P., Jones, A.R. and Antczak, P., 2020. Identifying robust biomarkers of infection through an omics-based meta-analysis. medRxiv.

## Batch correction

Removing batch correction from merged study datasets. PCA visualisation of removal of clustering by platform (batch effects) using our multistep batch correction pipeline:

![alt text](https://raw.githubusercontent.com/ashm97/Developing-an-infection-state-predictive-model/main/images/preview_batch_pca.png) 



## Backwards elimination

![alt text](https://raw.githubusercontent.com/ashm97/Developing-an-infection-state-predictive-model/main/images/example_backward_elim.png) 

## Genetically inspired search algorithm (GALGO)

** package currently unsuported by R 3.6

Victor Trevino, Francesco Falciani, GALGO: an R package for multivariate variable selection using genetic algorithms, Bioinformatics, Volume 22, Issue 9, 1 May 2006, Pages 1154–1156, https://doi.org/10.1093/bioinformatics/btl074

