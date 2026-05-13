# IPL Match Winner Prediction using Machine Learning

## Project Overview

This project focuses on analyzing IPL ball-by-ball cricket data and building machine learning models to predict match-winning outcomes using historical match information and engineered cricket features.

The project includes:
- Exploratory Data Analysis (EDA)
- Data preprocessing and feature engineering
- Model training and evaluation
- Comparative analysis of multiple ML models
- Prediction pipeline preparation
- Visual analytics for model interpretation

---

## Project Structure

```bash
project/
│
├── data/
│   └── ball_by_ball_ipl.csv
│
├── notebooks/
│   ├── dataprep.ipynb
│   ├── modeltraining.ipynb
│   └── prediction.ipynb
│
├── visuals/
│   ├── top_bowlers.png
│   ├── feature_importance_rf.png
│   ├── xgb_feature_importance.png
│   ├── rf_confusion_matrix.png
│   ├── xgb_roc_auc_curve.png
│   └── model_performance_comparison.png
│
├── saved_models/
│   ├── decision_tree_model.pkl
│   ├── random_forest_model.pkl
│   ├── xgboost_model.pkl
│   └── label_encoder.pkl
│
├── README.md
└── requirements.txt
```

---

## Workflow

### 1. Data Preparation
Notebook: `dataprep.ipynb`

Tasks performed:
- Data cleaning
- Missing value handling
- Feature engineering
- Leakage removal
- Group-aware train-test split
- Preparation of X and y datasets

---

### 2. Model Training
Notebook: `modeltraining.ipynb`

Models implemented:
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

---

### 3. Prediction Pipeline
Notebook: `prediction.ipynb`

Purpose:
- Load trained models
- Load preprocessing artifacts
- Generate predictions on unseen data
- Decode predicted classes into team names

---

## Key Insights

- Leakage-free training pipeline implemented using grouped match splitting
- Random Forest and XGBoost significantly outperformed a basic Decision Tree
- XGBoost achieved the best balanced multiclass performance
- Feature importance analysis revealed influential match-related features

---

## Model Performance Summary

| Model | Accuracy | Macro F1 Score |
|-------|----------|----------------|
| Decision Tree | ~39% | ~0.40 |
| Random Forest | ~50% | ~0.47 |
| XGBoost | ~48% | ~0.51 |

---

## Visualizations Included

- Top bowlers by wickets
- Feature importance plots
- Confusion matrix
- ROC-AUC curves
- Model performance comparison charts

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## Installation

Clone the repository:

```bash
git clone <repository-url>
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Live match win probability prediction
- Advanced feature engineering
- Deployment using Flask or Streamlit

---

## Author

Nitin Singh