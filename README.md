**Breast Cancer Classification Analysis
**Overview

This repository contains a machine learning project designed to classify breast tumors as Malignant or Benign. Using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset, I built a Logistic Regression model that analyzes 30 different cell nuclei measurements to provide a highly accurate diagnostic prediction.
Performance Metrics

The model achieved the following results on the test set:

    Accuracy: 97.66%

    AUC Score: 0.9977

    Confusion Matrix: * 102 Benign samples correctly identified (1 misclassified).

        65 Malignant samples correctly identified (3 misclassified).

**Dataset**

The dataset includes 569 samples with 30 quantitative features such as:

    Radius, Texture, and Perimeter

    Area and Smoothness

    Concavity and Symmetry Features are categorized by their Mean, Standard Error (se), and "Worst" (largest) values.

**Project Pipeline
**
    Data Cleaning: Handled headers, removed non-predictive IDs, and encoded diagnoses (M=1, B=0).

    Preprocessing: Used StandardScaler to normalize feature scales for the Logistic Regression algorithm.

    Modeling: Implemented LogisticRegression using Scikit-Learn with a 70/30 train-test split.

    Evaluation: Generated classification reports, confusion matrices, and ROC curves to validate reliability.

**Top Predictors
**
The analysis identified that the following features have the highest influence on predicting malignancy:

    texture_worst

    radius_se

    symmetry_worst

    area_se

    area_worst

**Technologies Used
**
    Language: Python

    Libraries: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

**Course**: CPE 4040

**Authors**: Anthony Nguyen & Steven Marsh (Team NaN Sense)
