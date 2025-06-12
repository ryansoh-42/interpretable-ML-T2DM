# Interpretable Modeling for Type 2 Diabetes Risk Factors

## Project Overview
This project explores the use of machine learning to predict the risk of Type 2 Diabetes, and identifying key contributing factors using health survey data.

**The objectives of this project includes the following:**
1. Predict whether an individual has Type 2 Diabetes using clinical and lifestyle features
2. Identify the important risk factors of Type 2 Diabetes using explainable machine learning
3. Provide a reproducible pipeline for public health research

**Important features used for prediction:**
- x
- y
- z

**Dataset used:**
- 

## Project Structure

```
interpretable-ML-T2DM/
│
├── data/                      # All data goes here (ignored in Git)
│   ├── raw/                   # Raw dataset files (not committed)
│   └── processed/             # Cleaned, merged datasets (ready for modeling)
│
├── notebooks/                # All research + analysis notebooks
│   ├── 01_data_overview.ipynb
│   ├── 02_cleaning_merging.ipynb
│   ├── 03_model_training.ipynb
│   ├── 04_shap_interpretability.ipynb
│   └── 05_results_summary.ipynb
│
├── src/                      # Modular scripts
│   ├── config.py             # Constants for paths, variable names
│   ├── preprocess.py         # Data cleaning and merging
│   ├── model.py              # Training and evaluation functions
│   └── explain.py            # SHAP/LIME interpretation code
│
├── report/                   # Paper-style results
│   └── summary_findings.pdf
│
├── requirements.txt          # Python packages
├── .gitignore                # Prevent committing data and artifacts
└── README.md                 # Project overview and instructions
```

## Setup Instructions


## License and Attribution
