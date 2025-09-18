# Credit Card Limit Guesser

## Introduction
The "Credit Card Limit Guesser" project aims to predict a customer's credit card limit based on their demographic and financial characteristics. This predictive model can assist financial institutions in assessing credit risk and allocating credit efficiently.

## Problem Formulation
We frame this as a supervised learning regression problem. The goal is to model the credit card limit as a function of customer features such as income, age, marital status, and education. The target variable, `credit_limit`, is continuous, making regression the appropriate choice.

## Dataset Description
The dataset used for this project contains information about customers and their credit card limits. Key details include:
- **Number of samples**: 10,000
- **Number of features**: Age, income, education, marital status, etc.
- **Label**: `credit_limit` (a continuous value)

### Preprocessing Steps
- Handle missing values.
- Normalize or scale numerical features.
- Encode categorical variables.

## Chosen ML Method
For Stage 1, we select **Linear Regression** as the initial machine learning model. This choice is justified because:
- The target variable (credit card limit) is continuous.
- Linear Regression is interpretable and provides a baseline for prediction accuracy.
- It allows us to understand the relationship between features and the target variable.

## Preliminary Analysis
- The distribution of `credit_limit` is right-skewed.
- Income shows a strong positive correlation with `credit_limit` (correlation coefficient ≈ 0.7).
- Age has a weak correlation with `credit_limit`.
- Outliers are present in features like income, which may require handling in preprocessing.

### Visualizations
- Histogram of `credit_limit`.
- Scatterplot of `income` vs. `credit_limit`.
- Boxplot of `credit_limit` grouped by categorical features (e.g., marital status).

## Plan for Stage 2
In the next stage, we will:
1. Experiment with additional ML methods such as Decision Trees and Support Vector Machines.
2. Compare the performance of these models using metrics like Mean Squared Error (MSE) and R-squared.
3. Perform hyperparameter tuning to optimize model performance.
4. Evaluate the models on a test set to ensure generalization.

---

This `README.md` serves as the foundation for the "Credit Card Limit Guesser" project, outlining the problem, dataset, chosen method, and preliminary findings. Further stages will build upon this groundwork to refine the model and improve predictions.
