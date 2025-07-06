# Interpretable Modeling for Type 2 Diabetes Risk Factors

## Project Overview
This project explores the use of machine learning models to predict the risk of Type 2 Diabetes, and identifying key contributing factors using health survey data and lab data.

**The objectives of this project includes the following:**
1. Predict whether an individual has Type 2 Diabetes using clinical and lifestyle features, classifying them into one of the three categories - diabetic, non-diabetic or borderline diabetic
2. Identify the important risk factors of Type 2 Diabetes using explainable machine learning
3. Assess whether an ensemble of machine learning models can significantly improve metric scores, compared to using standalone models

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
n.b. There are other variables that can influence a model's prediction.

**Dataset used:**
- All data used were contributed by the Centers for Disease Control and Prevention. The specific datasets used for model training and evaluation are from the NHANES August 2021 to August 2023 database.

## Project Structure

```
interpretable-ML-T2DM/
│
├── data/                      # All data goes here (ignored in Git)
│   ├── raw/                   # Raw dataset files (not committed)
│   ├── interim/               # Cleaned, merged datasets (ready for EDA)
│   ├── processed/             # Pre-processed datasets (ready for model training)
│   └── results/               # Stored results from model training (ready for comparison)
│
├── models/                    # All built models in 04_model_training.ipynb are saved here for analysis in the later notebooks
│   ├── adaboost_model.pkl
│   ├── decision_tree_model.pkl
│   ├── k-nearest_neighbors_model.pkl
│   ├── logistic_regression_model.pkl
│   ├── neural_network.keras
│   ├── random_forest_model.pkl
│   ├── support_vector_machine_model.pkl
│   └── xgboost_model.pkl
│
├── notebooks/                 # End-to-end analysis pipeline
│   ├── 01_data_cleaning_merge.ipynb
│   ├── 02_eda.ipynb
|   ├── 03_preprocessing.ipynb
│   ├── 04_model_training.ipynb
│   ├── 05_interpretability.ipynb
│   ├── 06_results_comparison.ipynb
│   └── 07_stacked_ensemble.ipynb
│
├── report/                    
│   ├── figures/               # All plot visualisations
│   └── report.pdf             # Paper-style report
│
├── requirements.txt           # Python packages
├── .gitignore                 # Prevent committing data and artifacts
└── README.md                  # Project overview and instructions
```

## Setup Instructions
### Clone the repository
```bash
git clone https://github.com/ryansoh-42/interpretable-ML-T2DM.git
cd interpretable-ML-T2DM
```

### Create and activate virtual environment
```bash
python3 -m venv venv
source venv\Scripts\activate # On Windows
source venv/bin/activate # On MacOS
```

### Install dependencies
```bash
pip install -r requirements.txt
```

**Dataset Access**
Please download the required datasets highlighted above from CDC NHANES website. You may find them here (https://wwwn.cdc.gov/nchs/nhanes/search/datapage.aspx?Component=Examination&Cycle=2021-2023)

## License and Attribution
This project uses publicly available datasets from the CDC NHANES survey and is intended solely for educational and research purposes.
Data source :  https://wwwn.cdc.gov/nchs/nhanes/search/datapage.aspx?Component=Examination&Cycle=2021-2023