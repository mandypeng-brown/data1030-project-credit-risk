# Credit Default Risk Prediction

This repository contains my final project for Brown University's DATA 1030 course. The project focuses on predicting whether a loan applicant will default using application-level data and historical loan records.

## Project Overview

- **Problem type:** Binary classification (default vs. non-default)
- **Goal:** Predict loan default risk to support better credit risk assessment
- **Dataset:** Kaggle Home Credit Default Risk
- **Scale:** 300K+ applicants, 134 original features
- **Main challenge:** severe class imbalance and substantial missing data

This project combines exploratory data analysis, preprocessing, feature engineering, model training, evaluation, and interpretability analysis in a reproducible notebook-based workflow.

## Key Highlights

- Merged application data with historical loan records to improve predictive power
- Conducted EDA on class imbalance, missingness, and major predictive signals
- Built preprocessing pipelines tailored to different model families
- Trained and compared multiple machine learning models
- Selected **XGBoost** as the best-performing model
- Used SHAP and error analysis to interpret global feature importance and local prediction behavior

## Main Findings

- Loan default is a rare event, making evaluation strategy and threshold selection especially important
- External credit scores were among the strongest predictors of default risk
- Historical behavior, such as previous refusals, added meaningful predictive value
- XGBoost achieved the best overall performance among the tested models
- Interpretability analysis showed that external credit scores, income stability, and loan magnitude were important drivers of predictions

## Recommended Starting Point

If you are reviewing this project for a quick overview, I recommend starting with:
**`slides/Final Presentation Slides.pdf`** – concise summary of the motivation, methods, results, and interpretation

## Repository Structure

- `src/` – main project notebooks for data merging, EDA, feature definition, training, and evaluation
- `figures/` – exported plots and visual outputs
- `results/` – saved outputs and intermediate results
- `slides/` – midterm and final presentation slides

## Methods

The project includes:

- stratified data splitting
- missing-value handling for numerical and categorical features
- preprocessing pipelines for linear and tree-based models
- model comparison across multiple classifiers
- threshold tuning for downstream decision-making
- SHAP-based interpretability and local error analysis

## Notes

Some large raw data files are not included in this public repository. This repository is intended to showcase the project workflow, methodology, and presentation materials.

## Author

Yumeng Peng  
Brown University, M.S. in Data Science
