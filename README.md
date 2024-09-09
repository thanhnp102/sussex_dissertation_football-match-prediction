# Predicting Football Match Results with Machine Learning Approaches Using Expected Goals (xG)

This repository contains the code, data, and documentation for the dissertation project titled "Predicting Football Match Results with Machine Learning Approaches Using Expected Goals". The primary goal of this project is to leverage Expected Goals (xG) values to improve football match outcome predictions using various machine learning algorithms.

## Table of Contents
- [Project Overview](#project-overview)
- [Datasets](#datasets)
- [Methodology](#methodology)
- [Models Used](#models-used)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Installation and Usage](#installation-and-usage)

## Project Overview
In recent years, football analytics has gained massive popularity. This project investigates the use of machine learning algorithms, incorporating Expected Goals (xG) values, to predict football match outcomes. xG values provide a quantitative measure of scoring opportunities, offering an advanced feature for predicting match results.

## Datasets
The dataset used in this project includes match statistics such as goals, shots, possession, fouls, and xG values. Data sources:
- **Wyscout Event Data**: For granular event-level data.
- **Football-data.co.uk**: For historical match statistics and betting odds.
- **Understat**: For pre-aggregated xG values.

## Methodology
The project follows a systematic approach:
1. Data Preprocessing
2. Feature Engineering (including xG values)
3. Model Training
4. Model Evaluation

The data is split into training and test sets, and various machine learning algorithms are applied to predict the outcomes of football matches (Home Win, Draw, or Away Win).

## Models Used
The following models were trained and compared:
- **Logistic Regression**
- **Support Vector Machines (SVMs)**
- **Random Forest**
- **Artificial Neural Networks (ANN)**
  
Each model was evaluated using both aggregated xG values from Understat and xG values predicted by our Expected Goals model.

## Evaluation Metrics
The models were evaluated based on several metrics:
- **Accuracy**
- **Precision, Recall, and F1 Score**
- **Log Loss**
- **Brier Score**
- **ROC AUC**
- **Calibration Curve**

## Results
- The Random Forest model showed the greatest improvement in accuracy when incorporating xG values.
- Logistic Regression had the most well-calibrated predictions.
- The models were compared to bookmakers’ odds for a baseline evaluation.
- Full results are provided in the ***Result*** section of the documentation.

## Installation and Usage

### Prerequisites
To run the project, ensure you have the following installed:
- Python 3.7+
- Jupyter Notebook
- Required libraries: scikit-learn, imbalanced-learn, numpy, pandas, matplotlib, seaborn, shap, tensorflow
