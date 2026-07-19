# NTs-LBN

# Multivariate Neurotransmitter Analysis

This repository contains the multivariate statistical analyses and machine learning workflows used to investigate the effects of Limited Bedding and Nesting (LBN) on neurotransmitter profiles in juvenile and adult mice.

The analyses include data preprocessing, dimensionality reduction, clustering, and predictive machine learning models.

---

## Repository Contents

### 1. `Multivariate_Analysis_Juvenile_without_interpolation.ipynb`

Performs the complete multivariate analysis on the juvenile dataset using only complete observations (no missing value imputation).

#### Workflow

- Import required Python libraries
- Load and inspect the dataset
- Data cleaning and preprocessing
- Removal of metabolites with excessive missing values
- Standardization of neurotransmitter concentrations
- Principal Component Analysis (PCA)
- Hierarchical Clustering (HC)
- Logistic Regression
- Random Forest classification
- Feature importance and model evaluation

This notebook is intended to evaluate the robustness of the analyses without introducing imputed values.

---

### 2. `Multivariate_Analysis_Juvenile_interpolation_Machine_Learning.ipynb`

Performs the same multivariate analyses on the juvenile dataset, but includes missing value imputation before machine learning.

#### Workflow

- Data import and inspection
- Data cleaning
- Missing value imputation using the median
- Feature scaling
- Principal Component Analysis (PCA)
- Hierarchical Clustering (HC)
- Logistic Regression
- Random Forest
- Hyperparameter optimization
- Model performance evaluation
- Feature importance analysis

This notebook allows comparison between analyses performed with and without missing value interpolation.

---

### 3. `Multivariate_Analysis_Adult_Machine_Learning.ipynb`

Performs the multivariate analysis on the adult dataset.

#### Workflow

- Import libraries
- Load adult neurotransmitter dataset
- Data quality assessment
- Cleaning and preprocessing
- Missing value handling
- Feature scaling
- Principal Component Analysis (PCA)
- Hierarchical Clustering (HC)
- Logistic Regression
- Random Forest classification
- Hyperparameter tuning
- Model evaluation and interpretation

---

## Datasets

The notebooks require the following Excel files:

### Juvenile analyses

```
Pups_Analyse NTs_221124.xlsx
```

### Adult analyses

```
Veave - Analyse NTs_Adult_230126-R.xlsx
```

These datasets are not included in this repository and should be placed in the same directory as the notebooks or the file paths should be updated accordingly.

---

## Required Python Packages

The notebooks make use of the following libraries:

- numpy
- pandas
- matplotlib
- seaborn
- scipy
- scikit-learn
- scikit-optimize (skopt)
- xgboost
- shap
- openpyxl
- torch (optional)

Most dependencies are installed automatically at the beginning of each notebook.

---

## Objectives

The purpose of these analyses is to determine whether neurotransmitter profiles can distinguish Control (CONT) and Limited Bedding and Nesting (LBN) animals using multivariate statistical approaches and supervised machine learning.

The notebooks investigate:

- Neurotransmitter profile variation
- Dimensionality reduction using PCA
- Sample clustering
- Classification performance
- Identification of the most informative neurotransmitters

---

## Reproducibility

To reproduce the analyses:

1. Clone the repository.
2. Install the required Python packages.
3. Place the appropriate Excel dataset(s) in the project directory.
4. Run the notebooks from top to bottom.

---

## Author

Lydia SRINIVASSAN

Master 1 student in Bioinformatics, GENIOMHE-AI

Internship Project
