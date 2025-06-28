# Titanic Survival Prediction using Logistic Regression

This project applies **Logistic Regression** to predict passenger survival on the Titanic using the classic [Titanic dataset](https://www.kaggle.com/c/titanic).

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [References](#references)

## Overview

The goal is to build a predictive model that determines whether a passenger survived the Titanic disaster based on features such as age, sex, class, and fare.

## Dataset

- Source: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic/data) or you can use from seaborn.
- Features: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`, etc.
- Target: `Survived` (0 = No, 1 = Yes)

## Results

- Model accuracy, confusion matrix, and classification report are displayed after training.
- Example output:
  ```
  Accuracy: 0.80
  ```

## References

- [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- [Logistic Regression - scikit-learn Documentation](https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression)
