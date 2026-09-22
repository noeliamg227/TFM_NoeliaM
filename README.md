# Machine learning approaches to predict recurrencerisk and characterize breast cancer patients

This repository contains the code used to develop and evaluate machine learning models for the prediction of clinically relevant breast cancer outcomes and clinicopathological characteristics.

## Overview

The study included 178 patients with invasive breast carcinoma of no special type, using integrated clinicopathological and immune profiling data obtained from the primary tumor and non-metastatic axillary lymph nodes (ALN−). Eleven immune cell populations, together with established clinical variables, were considered as predictive features.

Separate binary classification models were developed for four outcomes:

- Breast cancer recurrence: recurrence vs. non-recurrence
- Tumor diameter: ≤20 mm vs. >20 mm
- Age at diagnosis: ≤60 years vs. >60 years
- Molecular subtype: luminal vs. non-luminal

The analyses include feature selection, model development, cross-validation, performance evaluation, and feature interpretation.
Detailed methodological information is provided in the accompanying manuscript.

## Repository structure
```text
├── code/
│   ├── Recurrence.ipynb
│   ├── Tumor_Diameter.ipynb
│   ├── Age_at_diagnosis.ipynb
│   └── Molecular_Subtype.ipynb
│
├── data/                         # Not publicly available
│   └── [restricted dataset]
│
├── results/                      # Generated analysis outputs
│
└── README.md
```
The repository currently contains the `code/` directory. The study dataset is not publicly available due to privacy and ethical considerations. The `results/` directory represents the location where analysis outputs are generated when the notebooks are executed.

## Requirements

The analyses were developed using Python 3.11.4

Main Python packages include:

- numpy
- pandas
- scipy
- scikit-learn
- matplotlib
- shap

The required packages can be installed using:

pip install numpy pandas scipy scikit-learn matplotlib shap


## Clone the repository:

git clone <[repository-url](https://github.com/noeliamg227/TFM_NoeliaM.git)>

cd Project

The notebooks use relative paths to access the `data/` and `results/` directories. Therefore, the repository structure should be preserved.

Open the desired notebook from the `code/` directory using Jupyter Notebook:

jupyter notebook

Then select the corresponding notebook:

- Recurrence.ipynb
- Tumor_Diameter.ipynb
- Age_at_diagnosis.ipynb
- Molecular_Subtype.ipynb


## Data availability

The data supporting the findings of this study are not publicly available due to privacy and ethical considerations regarding the research participants. However, the data may be obtained from the corresponding author (AF-C) upon reasonable request.


## Citation

If you use this code or methodology, please cite the corresponding publication:

[Publication citation to be added once the manuscript is published.]
