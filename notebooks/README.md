# IPL Match Data Analysis & Machine Learning Pipeline

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA), preprocessing, feature engineering, and building a machine learning pipeline using IPL ball-by-ball cricket data.

The current stage of the project includes:
- Data cleaning
- Missing value handling
- Team and venue standardization
- Feature engineering
- Exploratory visualizations
- Processed dataset generation for ML training

The upcoming phase will include:
- Model training
- Evaluation
- Hyperparameter tuning
- Model comparison
- Match outcome prediction

---

# Dataset

The project uses IPL ball-by-ball match data containing:
- Match information
- Batting statistics
- Bowling statistics
- Venue details
- Match outcomes

---

# Project Structure

```text
AIPremierLeague/
│
├── data/
│   ├── ball_by_ball_ipl.csv
│   │
│   └── processed/
│       ├── X.csv
│       └── y.csv
│
├── notebooks/
│   ├── dataprep.ipynb
│   └── model_training.ipynb
│
├── visuals/
│
├── saved_models/
│
├── requirements.txt
│
└── README.md