# Cervical Cancer Multi-omics Machine Learning

This repository contains the code and resources for the research project on "Multi-omic data in cervical cancer studies using machine learning." The aim of this research is to help the medical society identify cervical cancer subtypes using multi-omics data of the patients.

## Aim and Objectives

### Aim
The aim of our research is to help the medical society identify the cervical cancer subtypes using multi-omics data of the patients.

### Objectives
1. To study the factors that could influence the performance of each machine learning method and create an accurate machine learning model for predicting the subgroup of cervical cancer patients.
2. To study the influence of different features on predicting the subgroups of cervical cancer.
3. To study the difference between omic data and build a more accurate machine learning model by taking advantage of using multi-omic data instead of single-omic data.

## Data Source
We utilize the TCGA (The Cancer Genome Atlas) data for our research. The following omics data are used in our analysis:
- miRNA Genome Data
- Gene Expression Profiling Data
- DNA Methylation Data

## Repository Structure
├── data/ # Directory for storing TCGA data files
│ ├── miRNA/ # Directory for miRNA genome data
│ ├── gene_expression/ # Directory for gene expression profiling data
│ └── DNA_methylation/ # Directory for DNA methylation data
│
├── notebooks/ # Jupyter notebooks for data preprocessing and analysis
│ ├── 01_data_preprocessing.ipynb
│ ├── 02_feature_selection.ipynb
│ ├── 03_model_training.ipynb
│ └── 04_evaluation.ipynb
│
├── models/ # Trained machine learning models
│
├── src/ # Source code for utility functions and modules
│ ├── data_loader.py
│ ├── feature_selection.py
│ ├── model.py
│ └── evaluation.py
│
├── README.md # Project overview and instructions
└── requirements.txt # Python dependencies

├── data/                # Directory for storing TCGA data files
│   ├── miRNA/           # Directory for miRNA genome data
│   ├── gene_expression/ # Directory for gene expression profiling data
│   └── DNA_methylation/ # Directory for DNA methylation data
│
├── notebooks/           # Jupyter notebooks for data preprocessing and analysis
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_feature_selection.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_evaluation.ipynb
│
├── models/              # Trained machine learning models
│
├── src/                 # Source code for utility functions and modules
│   ├── data_loader.py
│   ├── feature_selection.py
│   ├── model.py
│   └── evaluation.py
│
├── README.md            # Project overview and instructions
└── requirements.txt     # Python dependencies


## Usage

1. Clone the repository:

   ```shell
   git clone https://github.com/your-username/cervical-cancer-multiomics-machine-learning.git



