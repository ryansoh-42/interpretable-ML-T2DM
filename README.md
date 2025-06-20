# Interpretable Modeling for Type 2 Diabetes Risk Factors

## Project Overview
This project explores the use of machine learning method to predict the risk of Type 2 Diabetes, and identifying key contributing factors using health survey data and lab data.

**The objectives of this project includes the following:**
1. Predict whether an individual has Type 2 Diabetes using clinical and lifestyle features, classifying them into one of the three categories - diabetic, borderline diabetic or not diabetic
2. Identify the important risk factors of Type 2 Diabetes using explainable machine learning
3. Identify the presence of an ensemble of machine learning models that can significantly improve metric scores, compared to using individual models standalone
4. Provide a reproducible pipeline for public health research

**Important features used for prediction:**
1. BMI
2. History of high blood pressure
3. Gender
4. Age in years at screening
5. Glycohemoglobin level (HbA1c) (%)
6. Fasting Plasma Glucose level (FPG) (mmol/L)
7. High Density Lipoprotein (HDL) (mmol/L)
8. Current smoking frequency
9. Diabetic (target variable y)

**Dataset used:**
- All data used were contributed by the Centers for Disease Control and Prevention. The specific datasets used for model training and evaluation are from the NHANES August 2021 to August 2023 database.

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
|   ├── 03_preprocessing.ipynb
│   ├── 04_model_training.ipynb
│   ├── 05_shap_interpretability.ipynb
│   └── 06_results_summary.ipynb
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
