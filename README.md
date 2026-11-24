
# Course Cancellation Prediction | Machine Learning

## Project Overview

An end-to-end machine learning project designed to predict the probability of course registration cancellations at Nova Academy.

The project follows the CRISP-DM methodology, combining exploratory data analysis, data preprocessing, feature engineering, predictive modeling, and model interpretability to support data-driven business decisions.

## Business Objective

The main objective is to identify customers at high risk of cancelling their course registrations, enabling the academy to implement targeted retention strategies, improve resource allocation, and reduce potential revenue loss.

## Dataset

- Training dataset: 63,464 observations and 29 variables.
- Test dataset: 15,866 observations and 28 variables.
- Target variable: Dropped_Course (binary classification).
- Cancellation rate: approximately 41.4%.

The original datasets are not included in this repository due to data privacy and academic restrictions.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

- Statistical analysis and data visualization.
- Target variable distribution analysis.
- Correlation analysis.
- Identification of cancellation patterns.
- Detection of missing values, outliers, and data quality issues.

### 2. Data Preprocessing

- Missing value imputation.
- Categorical data standardization.
- Outlier detection and treatment.
- Categorical feature encoding.
- Numerical feature scaling.

### 3. Feature Engineering

- Creation of new predictive features.
- Transformation of existing variables.
- Identification of relevant customer and registration characteristics.

### 4. Machine Learning Models

Three classification algorithms were implemented and evaluated:

- Logistic Regression
- Random Forest
- XGBoost

Model optimization was performed using:

- Cross-Validation
- RandomizedSearchCV
- GridSearchCV
- Hyperparameter Tuning

## Model Performance

ROC-AUC was selected as the primary evaluation metric.

| Model | Cross-Validation ROC-AUC |
|---|---:|
| Logistic Regression (Baseline) | 0.8975 |
| Random Forest | 0.9243 |
| XGBoost (Randomized Search) | 0.9445 |
| XGBoost (Final Selected Model) | 0.9302 |

The final XGBoost configuration was selected with an emphasis on model stability and generalization.

Final hyperparameters:

- Learning rate: 0.1
- Maximum depth: 4
- Number of estimators: 150

Additional evaluation metrics included accuracy, precision, recall, F1-score, and confusion matrices.

## Model Explainability

Feature importance and SHAP (SHapley Additive exPlanations) were used to interpret the model's predictions and identify the key factors associated with cancellation risk.

## Key Business Insights

- Customers who register further in advance tend to have a higher cancellation risk.
- Previous course cancellations are strong predictors of future cancellations.
- Returning customers tend to have a lower cancellation risk.
- Longer waiting periods are associated with higher cancellation rates.
- Physical course kits are associated with a lower predicted cancellation risk.

These findings can support targeted customer retention initiatives and more informed operational decisions.

## Technologies & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- SHAP
- Jupyter Notebook
- Google Colab

## Repository Structure

- README.md - Project documentation
- course_cancellation_prediction.ipynb - Data analysis and machine learning implementation
- requirements.txt - Python dependencies
- .gitignore - Git configuration

## Data Availability

The original training and test datasets are not publicly distributed as part of this repository. Reproducing the model training and generating predictions requires access to the original datasets.

## Authors

Developed collaboratively by Gal and Aviv as part of an academic Machine Learning project at Tel Aviv University.
