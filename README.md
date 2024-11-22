# Wine Quality Prediction System 🍷

A machine learning project aimed at predicting the quality of wine based on its physicochemical properties. The project leverages various classification algorithms to classify wines as high-quality or low-quality, along with data preprocessing, feature engineering, and hyperparameter tuning.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Project Workflow](#project-workflow)
- [Algorithms Used](#algorithms-used)
- [Installation](#installation)
- [Results and Insights](#results-and-insights)
- [Future Enhancements](#future-enhancements)
- [Acknowledgments](#acknowledgments)

---

## Project Overview

Wine quality prediction is critical in the wine industry, where quality assessment is subjective and requires expertise. This project predicts wine quality using machine learning models, based on features such as acidity, sugar levels, pH, and alcohol content. The goal is to classify wines as **high-quality** (score ≥ 7) or **low-quality** (score < 7) based on physicochemical data.

---

## Dataset Information

The dataset used is the **Wine Quality Dataset** from the UCI Machine Learning Repository. It contains information on red wine samples with the following details:

- **Number of samples**: 1,599
- **Number of features**: 12

### Features:
- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol
- **Quality** (target variable)

---

## Project Workflow

### Data Preprocessing:
- Handling missing values.
- Renaming columns for better readability.
- Encoding categorical variables using `pd.get_dummies`.

### Exploratory Data Analysis (EDA):
- Visualizing feature distributions using histograms.
- Examining correlations using a heatmap.
- Bar plots to analyze the relationship between quality and features (e.g., alcohol content).

### Feature Engineering:
- Creating a binary target variable (`best quality`).
- Removing highly correlated features.
- Standardizing and normalizing features for better model performance.

### Model Building:
- Splitting the dataset into training and testing sets.
- Training models: **Logistic Regression**, **Decision Trees**, **Random Forest**, and **XGBoost**.
- Hyperparameter tuning using **GridSearchCV**.

### Model Evaluation:
- Evaluating accuracy, precision, recall, F1 score, and AUC-ROC.
- Confusion matrices to understand model predictions.

---

## Algorithms Used

The following algorithms were implemented and compared:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**
4. **XGBoost Classifier**

Each algorithm was optimized for accuracy and evaluated using cross-validation.

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/wine-quality-prediction.git
cd wine-quality-prediction

### 2. Installation Dependencies
