# BCF-Concentration-of-PFAS-in-plant

# Predicting Bioconcentration Factors and Concentrations of Per- and Polyfluoroalkyl Substances in Plants with Machine Learning
Official implementation of the paper "Predicting Bioconcentration Factors and Concentrations of Per- and Polyfluoroalkyl Substances in Plants with Machine Learning".

## Repository Overview

This repository contains the implementation and data for the paper "Predicting Bioconcentration Factors and Concentrations of Per- and Polyfluoroalkyl Substances in Plants with Machine Learning". It includes four machine learning models (XGBoost, Random Forest, MLP, SVR) for BCF and concentration prediction with comprehensive model interpretation using SHAP, permutation importance, and partial dependence plots.

### Repository Structure

├── ANN-BCF.ipynb # Artificial Neural Network model
├── RF-BCF.ipynb # Random Forest model
├── SVM-BCF.ipynb # Support Vector Machine model
├── XGBoost_BCF+feature importance.ipynb # XGBoost with feature importance
├── XGBoost-BCF-PDP.ipynb # XGBoost with Partial Dependence Plots
├── Data cleaning.ipynb # Data preprocessing and cleaning
├── PFAS-ECF.ipynb # ECFP fingerprint generation & visualization
├── data/ # Processed datasets
│ ├── dataset_concn.csv.csv # Preprocessed data for concentration
│ └── dataset_BCF.csv # Preprocessed data for BCF
├── requirements.txt # Python dependencies
└── README.md # This file

## Model Scope

This repository contains code for **BCF (Bioconcentration Factor) prediction models**. The same codebase can be used for **Concentration prediction** by simply modifying the file paths to point to concentration datasets. All modeling approaches, feature engineering, and interpretation methods are identical for both endpoints.

## Getting Started

### Prerequisites

- Python 3.11 or higher
- pip (Python package installer)
- Jupyter Notebook

### Installation & Setup

#### 1. Clone the Repository

```bash
git clone https://github.com/Rui488/BCF-Concentration-of-PFAS-in-plant.git
cd BCF-Concentration-of-PFAS-in-plant
```
#### 2. Setting Up Python Environment
If you don't have Python installed:

Windows: Download from python.org

macOS:
bash
# Using Homebrew
brew install python

Linux:
bash
# Ubuntu/Debian
sudo apt update
sudo apt install python3 python3-pip

If you don't have Jupyter installed:
bash
pip install jupyter

#### 3. Install Required Packages
bash
pip install -r requirements.txt
Troubleshooting Package Installation
If specific packages fail to install:

bash
# Install packages individually
pip install numpy pandas scikit-learn
pip install xgboost
pip install shap
pip install matplotlib seaborn
pip install tqdm scipy jupyter


### Reproducing Results
# 1. Data Preparation:

The data/ folder contains already preprocessed data ready for modeling

For transparency, we provide Data cleaning.ipynb and PFAS-ECFP.ipynb to show the data preprocessing and fingerprint generation steps we performed

# 2. Run Models:

Individual model notebooks:
ANN-BCF.ipynb
RF-BCF.ipynb
SVM-BCF.ipynb
XGBoost_BCF+feature importance.ipynb
XGBoost-BCF-PDP.ipynb

Starting Jupyter Notebook:
bash
jupyter notebook
Then open the desired .ipynb file from the browser interface.

### For Concentration Models
To adapt this code for Concentration prediction:
1. Replace BCF dataset files with Concentration datasets
2. Update file paths in the notebooks to point to your Concentration data
3. The same modeling and interpretation approaches apply directly


### License
This project is licensed under the MIT License - see the LICENSE file for details.

### Contact
[Rui Li] - [rui18752@gmail.com]
