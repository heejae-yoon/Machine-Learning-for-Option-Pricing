# Machine-Learning-for-Option-Pricing

## Introduction

The project, titled "Machine Learning - Option Pricing," focuses on predicting the value of European call options and classifying whether the option's value is overestimated or underestimated based on the Black-Scholes model. We used a combination of machine learning techniques, and all code for the analysis is provided in a single Python file.

## Repository Contents

1. **Option Pricing Report**: A detailed report explaining the entire project, from data exploration and analysis to model selection and final results.
2. **Option Pricing Code**: The Python code used for data analysis and model implementation. This file includes:
   - Data preprocessing, including outlier detection, standardization, and normalization.
   - Regression models to predict option values, including Linear Regression, KNN, LASSO, RIDGE, Decision Tree, and Random Forest.
   - Classification models to predict over/undervaluation, including Logistic Regression, KNN, Decision Tree, Random Forest, SVM, and XGBoost.

## Dataset Description

The dataset used in this project contains historical option pricing data for European call options on the S&P 500 index. Key variables include:
- **S**: Underlying asset price
- **K**: Strike price
- **tau**: Time to maturity
- **r**: Risk-free rate
- **Value**: Option value

The target variables for prediction are:
- **Value**: Option value.
- **BS**: A binary indicator of whether the Black-Scholes model overestimates or underestimates the option value.

## Summary of Findings

1. **Random Forest for Regression**: Among the models tested for predicting option values, Random Forest provided the highest prediction accuracy, with an out-of-sample R-squared of 99.69%. Its ability to handle non-linear relationships and avoid overfitting made it the best choice for regression.
   
2. **XGBoost for Classification**: For classifying whether the Black-Scholes model overestimates or underestimates the option price, XGBoost achieved the lowest mean classification error of 5.95%, making it the optimal choice for classification.

3. **Feature Importance**: The inclusion of all four predictor variables—S, K, tau, and r—was critical to maximizing model performance. Excluding any feature reduced prediction accuracy, underscoring their importance in the model.

## Conclusion

This project demonstrates how machine learning models can outperform traditional financial models like Black-Scholes by incorporating more data and adapting to changing market conditions. The Random Forest and XGBoost models delivered high accuracy in both option value prediction and classification of over/undervaluation.

---

For more detailed information, please refer to the project report included in this repository.
