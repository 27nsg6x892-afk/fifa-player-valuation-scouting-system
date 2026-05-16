# FIFA Player Valuation & Scouting System

## Overview
This project is a machine learning system for football player scouting. It predicts player market value and classifies player performance tier using player attributes and performance-related features.

The project includes a complete machine learning workflow: data loading, exploratory data analysis, preprocessing, feature engineering, model training, model comparison, cross-validation, and final inference testing.

## Objectives
- Predict football player market value
- Classify players into performance tiers
- Compare multiple regression and classification models
- Build a final scouting system that returns both predicted market value and predicted performance tier
- Evaluate model performance using suitable regression and classification metrics

## Dataset
The football player dataset contains 19,667 rows and 9 columns.

Main feature groups include:
- Player identity and categorical features such as country, position, and team
- Numerical features such as age, overall rating, future potential, and total stats score
- Regression target: player market value
- Classification target: performance tier

Note: The full dataset may be excluded from the repository if needed because of file size or usage limitations. A small sample can be included to show the expected data structure.

## Methods Used
- Data cleaning
- Exploratory Data Analysis
- Feature engineering
- One-hot encoding
- Feature scaling
- Train/test splitting
- Cross-validation
- Regression modeling
- Classification modeling
- Ensemble learning
- Final inference function

## Models Used

### Regression Models
- Lasso Regression
- Ridge Regression
- KNN Regressor
- SVM Regression
- Random Forest Regressor
- Voting Regressor Ensemble

### Classification Models
- Logistic Regression
- Naive Bayes
- KNN Classifier
- SVM Classifier
- Random Forest Classifier
- Voting Classifier Ensemble

## Results

### Final Regression Model
The final selected regression model was a Voting Regressor Ensemble.

- Test R²: 0.9757
- Test RMSE: 0.1193
- Cross-validation R² mean: 0.9681
- Cross-validation R² standard deviation: 0.0078

### Final Classification Model
The final selected classification model was an SVM Classifier.

- Test accuracy: 86.17%
- Test F1 macro: 0.8602
- Cross-validation accuracy mean: 0.8604
- Cross-validation accuracy standard deviation: 0.0050

## Example System Output
The final system can take a new player profile and return:
- Predicted market value
- Predicted performance tier

Example outputs from the project:
- Egypt, ST, age 24, overall 82, potential 86 → Predicted value: 38.16 M$, tier: Elite
- France, CM, age 21, overall 76, potential 88 → Predicted value: 15.47 M$, tier: Elite
- Brazil, LW, age 29, overall 89, potential 89 → Predicted value: 65.33 M$, tier: Elite

## Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Repository Structure
```text
fifa-player-valuation-scouting-system/
│
├── fifa_player_valuation_scouting.ipynb
├── fifa.pdf
├── requirements.txt
├── results.json
├── assignment2_summary.json
├── README.md
└── sample_data/
