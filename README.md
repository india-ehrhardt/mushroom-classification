# Mushroom Edibility Classification — Decision Tree & Random Forest

**Tools:** Python, pandas, scikit-learn, matplotlib  
**Course:** Data Analytics — Metropolitan State University of Denver

---

## Overview

Built and compared two machine learning classification models to predict whether a mushroom is poisonous or edible based on its physical characteristics. Given the high-stakes nature of misclassification (a false "edible" prediction could be dangerous), model accuracy and false negative rate were the primary evaluation criteria.

---

## What I Did

- **Data Preprocessing:** Loaded a dataset of ~60,000 mushroom samples; handled missing values by treating them as a separate category, and converted all categorical variables to dummy variables using one-hot encoding
- **Train/Test Split:** Divided data 70/30 into training and testing sets using stratified sampling to preserve class balance
- **Model 1 — Decision Tree:** Trained a Decision Tree classifier and visualized the full tree structure to understand how the model made decisions
- **Model 2 — Random Forest:** Trained a Random Forest ensemble of 100 decision trees to reduce overfitting and improve stability
- **Evaluation:** Assessed both models using accuracy scores and confusion matrices, focusing on false negatives as the highest-risk error type

---

## Results

| Model | Accuracy | False Negatives | False Positives |
|---|---|---|---|
| Decision Tree | 99.86% | 4 | 22 |
| Random Forest | **100%** | **0** | **0** |

The Random Forest model achieved perfect classification on the test set — zero poisonous mushrooms misclassified as edible.

---

## Key Findings

- The Decision Tree produced 4 false negatives (poisonous mushrooms classified as edible) — an unacceptable error for a consumer safety application
- The Random Forest eliminated all misclassifications by combining 100 decision trees, dramatically reducing variance and overfitting
- Random Forest was selected as the final model due to its 100% accuracy and zero false negatives

---

## Files

| File | Description |
|---|---|
| `project_1_india_ehrhardt.py` | Python script with full model implementation |
| `Project_1_India_Ehrhardt.ipynb` | Google Colab notebook version with step-by-step walkthrough |
| `Project_1_Report_India_Ehrhardt.pdf` | Business report summarizing methods, results, and model recommendation |

---

## Skills Demonstrated

`Python` `pandas` `scikit-learn` `Decision Tree` `Random Forest` `Confusion Matrix` `Model Comparison` `Classification` `Data Preprocessing` `matplotlib`

