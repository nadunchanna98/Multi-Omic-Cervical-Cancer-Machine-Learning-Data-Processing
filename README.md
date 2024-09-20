# Multi-Omic Data In The Cervical Cancer Study

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

This repository contains code and resources for the research project titled "Multi-omic Data in Cervical Cancer Studies using Machine Learning."

## Cervical Cancer Introduction

Cervical cancer is one of the most commonly diagnosed cancers affecting the cervix in women. The majority of cases are diagnosed between the ages of 20-29, peak between 55-64 years, and become rarer beyond the age of 65. The high mortality rate is often due to limited early detection techniques, especially in developing countries.

## Aim

- To identify cervical cancer subtypes using multi-omic data from patients.

## Scope

- Enhance machine learning models to identify cervical cancer subgroups more accurately.

## Dataset

We utilize the TCGA (The Cancer Genome Atlas) data for our research. The following omics are used:

| Omic             | Type               |
|------------------|--------------------|
| DNA Methylation  | Methylation450k     |
| Gene Expression  | Gene expression     |
| miRNA            | IlluminaHiseq       |

Please note that due to data privacy restrictions, the TCGA dataset cannot be included in this repository. 

## Cervical Cancer Subtypes

Based on the multi-omic data analysis, the cervical cancer cases can be classified into the following molecular subtypes in our dataset:

| Subtype                                      | Percentage | Number of Patients |
|----------------------------------------------|------------|--------------------|
| Adenosquamous                                | 2.244%     | 7                  |
| Cervical Squamous Cell Carcinoma             | 82.372%    | 257                |
| Endocervical Type of Adenocarcinoma          | 7.051%     | 22                 |
| Endocervical Adenocarcinoma of the Usual Type| 1.923%     | 6                  |
| Mucinous Adenocarcinoma of Endocervical Type | 5.449%     | 17                 |
| Endometrioid Adenocarcinoma of Endocervix    | 0.962%     | 3                  |

Cervical cancer can be categorized into the following main types based on the cells in which they originate:

### Adenocarcinoma

Adenocarcinoma starts in the glandular cells of the cervix, which are responsible for mucus production. It accounts for about **20% of cases**. The following subtypes are included under Adenocarcinoma:

- **Endocervical adenocarcinoma of the usual type**
- **Endocervical type of adenocarcinoma**
- **Endometrioid adenocarcinoma of endocervix**
- **Mucinous adenocarcinoma of endocervical type**  

### Squamous Cell Carcinoma

Squamous cell carcinoma is the **most common type** of cervical cancer, accounting for about **70% of cases**. It begins in the squamous cells, which are the flat cells lining the outer part of the cervix.

- **Cervical squamous cell carcinoma**

### Adenosquamous Carcinoma

Adenosquamous carcinoma is a rare type of cervical cancer, involving both squamous cells and glandular cells. These are also known as **mixed carcinomas**.

- **Adenosquamous carcinoma**

---

### Principal Component Analysis results (PCA)

## Visualization of the Main Cancer Types

Using PCA, we observed a clear separation between the two main cervical cancer types:

- **Adenocarcinoma**: This type forms its own cluster, distinct from Squamous Cell Carcinoma.
- **Squamous Cell Carcinoma**: This type also forms a separate cluster, with minimal overlap between the two.

This visualization helps confirm that the multi-omic data (DNA methylation, gene expression, and miRNA profiles) contains significant patterns that allow machine learning models to effectively distinguish between these cancer subtypes.


## Algorithms

Several machine learning algorithms were employed to classify cervical cancer subtypes based on multi-omic data. Below is a brief description of each:

- **Random Forest (RF)**:
  - A powerful ensemble learning method that constructs multiple decision trees and merges them to get a more accurate and stable prediction.
  
- **Support Vector Machine (SVM)**:
  - A supervised learning model used for classification tasks by finding the hyperplane that best separates the data into different classes.
  
- **K-Nearest Neighbor (KNN)**:
  - A non-parametric method that classifies instances based on the majority vote of their nearest neighbors.
  
- **Decision Tree (DT)**:
  - A simple and interpretable model that splits the data into subsets based on the feature that provides the most information gain.
  
- **eXtreme Gradient Boosting (XGB)**:
  - An efficient and accurate ensemble method that builds additive models in a forward stage-wise manner, optimizing differentiable loss functions.

Each of these algorithms was tuned and evaluated using performance metrics such as accuracy, precision, recall, and F1-score to determine the best-performing model.

## Repository Structure

The repository is organized as follows:

- `data_preparation/`: Code and instructions for accessing and preprocessing the TCGA data.
- `feature_selection/`: Code for feature selection and analysis.
- `model_training/`: Code for training machine learning models using multi-omic data.
- `evaluation/`: Code for evaluating the performance of the models.
- `results/`: Directory to store the results and outputs generated during the research.
- `references/`: Relevant papers and articles used for literature review.

## Requirements

To run the code in this repository, you will need the following dependencies:

- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- XGBoost

Please refer to the individual directories for specific requirements and installation instructions.

## References

- **The Cancer Genome Atlas**: [https://cancergenome.nih.gov](https://cancergenome.nih.gov)
- **Random Forest Algorithm**: Breiman, L. (2001). Random Forests. *Machine Learning*, 45(1), 5-32.
- **Support Vector Machines**: Cortes, C., & Vapnik, V. (1995). Support-vector networks. *Machine Learning*, 20(3), 273-297.
- **K-Nearest Neighbor Algorithm**: Cover, T., & Hart, P. (1967). Nearest neighbor pattern classification. *IEEE Transactions on Information Theory*, 13(1), 21-27.
- **Decision Trees**: Quinlan, J. R. (1986). Induction of decision trees. *Machine Learning*, 1(1), 81-106.
- **eXtreme Gradient Boosting**: Chen, T., & Guestrin, C. (2016). XGBoost: A scalable tree boosting system. In *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining* (pp. 785-794).

## Contributors

- [Nadun Channa](https://github.com/nadunchanna98)
- [Ruvindya Sachinthani](https://github.com/Ruvindya)
