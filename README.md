# Predicting Insulin Resistance-related genes using Biomedical Knowledge Graphs

This repository contains the code and data used in the study "Predicting Insulin Resistance-related genes using Biomedical Knowledge Graphs". The study explores the application of knowledge graph feature engineering approaches to biomedical knowledge graphs for the purpose of identifying novel gene-disease associations and gaining a better understanding of disease biology.

## Background

The study focuses on the use of topological metrics and embeddings to analyze biomedical knowledge graphs, specifically those related to insulin resistance. The study uses the OpenBioLink and Hetionet biomedical knowledge graphs to predict insulin resistance-related genes using various algorithms, including positive unlabelled learning and outlier detection algorithms.

## Data

The data used in the study includes the OpenBioLink and Hetionet biomedical knowledge graphs, as well as the DepMap dataset and Multiscale Interactome biomedical knowledge graph for biological characterization. The study also uses bioinformatic pathway functional annotations.

## Results

The study found that models using topological features from both standard and enriched OpenBioLink achieved the top predictive performances across various calculated metrics, followed closely by the positive unlabelled learning method using RotatE embeddings from both enriched and standard biomedical knowledge graphs. However, for the specific purpose of identifying genes related to insulin resistance, the model with the best hits@100 was RotatE on the enriched OpenBioLink.

Additionally, the study found that a larger training set had a stronger effect on performance than enrichment of the biomedical knowledge graphs without the need for modifying their schemas. The biological characterization showed that embeddings can capture the varied insulin resistance-related functions and broadly group them according to their relation to cell proliferation and metabolism. The enriched functional pathways of the top predicted genes included Chagas disease and toxoplasmosis, which have a debated relation to insulin resistance.

## Results
The study found that models using topological features from both standard and enriched OpenBioLink achieved the top predictive performances across various calculated metrics, followed closely by the positive unlabelled learning method using RotatE embeddings from both enriched and standard biomedical knowledge graphs. However, for the specific purpose of identifying genes related to insulin resistance, the model with the best hits@100 was RotatE on the enriched OpenBioLink.

The study comprehensively evaluated methods for identifying genes related to the complex patho-phenotype of insulin resistance. The findings showed that biomedical knowledge graph embeddings can capture complex biological information related to insulin resistance, without strong dependence on the specific schema of the knowledge graph. Comparing biologically contextualized results, the study found that embedding-based models had better generalization capabilities than the topology-based model, but there was a wide range of performance across the embedding-based models. Therefore, choosing an approach should balance the need for accurate predictions and the possibility of discovering novel biological insights.

## Code

The code used in the study is included in this repository. The code includes scripts for data preprocessing, feature engineering, and model training and evaluation. The code is written in Python and uses several libraries, including PyKeen, PyTorch, scikit-learn, and NetworkX. The code is organized into several Jupyter notebooks, each corresponding to a specific task in the study.

## License

This repository is licensed under the MIT License. See the LICENSE file for details.
