# Early Prediction of Breast Cancer Recurrence Using Machine Learning


This repository contains the code and supporting files used for the machine learning analyses described in the study on the early prediction of breast cancer recurrence using clinicopathological and immune-cell features from primary breast tumors and axillary lymph nodes without detectable metastasis (ALN−).

## Overview

The study investigates whether machine learning models can identify patients at higher risk of breast cancer recurrence within 120 months using clinical, pathological, and immune-related features available at diagnosis.

Three analytical approaches were investigated:

Age at diagnosis
Molecular subtype
Tumor diameter

The analyses include feature selection, model development, cross-validation, performance evaluation, and feature interpretation.

## Repository structure
Project/
│
├── code/
│   ├── Age_at_diagnosis_GITHUB.ipynb
│   ├── MolecularSubtype_GITHUB.ipynb
│   └── TumorDiameter_GITHUB.ipynb
│
├── data/
│   └── Base mama FIS 2012-2014 TOR TGN Para IA.csv
│
├── results/
│   ├── Age_at_diagnosis/
│   ├── MolecularSubtype/
│   └── TumorDiameter/
│
└── README.md

### code/

Contains the Jupyter notebooks used to perform the analyses.

Age_at_diagnosis_GITHUB.ipynb: analysis according to age at diagnosis.
MolecularSubtype_GITHUB.ipynb: analysis according to molecular subtype.
TumorDiameter_GITHUB.ipynb: analysis focused on tumor diameter.
data/

Contains the dataset required to reproduce the analyses.

The dataset includes clinicopathological and immune-cell variables used for model development and evaluation.

Data availability: The dataset may contain patient-level clinical information and therefore may not be publicly distributable. If the dataset cannot be shared publicly, this directory should be omitted from the public repository and the README should describe how eligible researchers can request access.

### results/

Contains the outputs generated during the analyses, including model performance results, selected features, and other analysis outputs.

## Methods

The machine learning workflow included:

Data loading and preprocessing.
Handling of missing values.
Definition of the recurrence outcome within 120 months.
Feature selection using Recursive Feature Elimination with Cross-Validation (RFECV).
Random Forest model development.
Stratified train/test splitting and cross-validation.
Model performance evaluation using:
Area Under the Receiver Operating Characteristic Curve (AUC)
Accuracy
Recall
Feature interpretation using SHAP values.
Evaluation across multiple stratified data splits to assess model variability.

Detailed methodological information is provided in the accompanying manuscript.

## Requirements

The analyses were developed using Python 3.9.

Main Python packages include:

numpy
pandas
scikit-learn
matplotlib
shap
tqdm

The required packages can be installed using:

pip install numpy pandas scikit-learn matplotlib shap tqdm
Running the analyses

## Clone the repository:

git clone <repository-url>
cd Project

The notebooks use relative paths to access the data and results directories. Therefore, the repository structure should be preserved.

Open the desired notebook from the code/ directory using Jupyter Notebook or JupyterLab:

jupyter notebook

Then select the corresponding notebook:

Age_at_diagnosis_GITHUB.ipynb
MolecularSubtype_GITHUB.ipynb
TumorDiameter_GITHUB.ipynb
Reproducibility

Random seeds are specified in the analysis code to facilitate reproducibility.

The analyses use repeated stratified train/test splits and cross-validation. Due to the stochastic nature of some machine learning procedures and differences between software versions or computational environments, minor differences in numerical results may occur.

## Ethical considerations and data protection

The study was conducted using previously collected clinical data in accordance with the applicable ethical and data protection requirements. Patient-level data should not be redistributed through this repository unless appropriate authorization and anonymisation requirements are satisfied.

## Citation

If you use this code or methodology, please cite the corresponding publication:

[Publication citation to be added once the manuscript is published.]

## Contact

For questions regarding the code or methodology, please contact the corresponding author of the associated publication.
