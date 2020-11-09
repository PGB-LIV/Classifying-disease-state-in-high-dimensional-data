# Developing-an-infection-state-predictive-model

This repository contains code supporting the study from https://www.medrxiv.org/content/10.1101/2020.07.28.20163329v2. 

## Abstract

A fundamental problem for disease treatment is that while antibiotics are a powerful counter to bacteria, they are ineffective against viruses. Often, bacterial and viral infections are confused due to their similar symptoms and lack of rapid diagnostics. With many clinicians relying primarily on symptoms for diagnosis, overuse and misuse of modern antibiotics are rife, contributing to the growing pool of antibiotic resistance. To ensure a given individual receives optimal treatment given their disease state and to reduce over-prescription of antibiotics, the host response can be measured quickly to distinguish between the two states. To establish a predictive biomarker panel of disease state (viral/bacterial/no-infection) we conducted a meta-analysis of human blood infection studies using Machine Learning (ML). We focused on publicly available gene expression data from two widely used platforms, Affymetrix and Illumina microarrays as they represented a significant proportion of the available data. We were able to develop multi-class models with high accuracies with our best model predicting 93% of bacterial and 89% viral samples correctly. To compare the selected features in each of the different technologies, we reverse engineered the underlying molecular regulatory network and explored the neighbourhood of the selected features. This highlighted that although on the gene-level the models differed, they did contain genes from the same areas of the network. Specifically, this convergence was to pathways including the Type I interferon Signalling Pathway, Chemotaxis, Apoptotic Processes, and Inflammatory / Innate Response. 

If used please cite: Myall, A.C., Perkins, S., Rushton, D., Jonathan, D., Spencer, P., Jones, A.R. and Antczak, P., 2020. Identifying robust biomarkers of infection through an omics-based meta-analysis. medRxiv.

## Preview

![alt text](https://github.com/[ashm97]/[Developing-an-infection-state-predictive-model]/images/preview_batch_pca.png?raw=true)
