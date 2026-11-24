
# Course Cancellation Prediction | Machine Learning

## Project Overview

An end-to-end machine learning project designed to predict the probability of course registration cancellations at Nova Academy.

The project follows the CRISP-DM methodology, combining exploratory data analysis, data preprocessing, feature engineering, predictive modeling, and model interpretability to support data-driven business decisions.

## Business Objective

The primary objective is to identify customers at high risk of cancelling their course registrations, enabling the academy to:

- Implement targeted customer retention strategies.
- Reduce course cancellation rates.
- Minimize potential revenue loss.
- Improve operational planning and resource allocation.
- Support data-driven decision-making.

## Dataset

- Training dataset: 63,464 observations.
- Target variable: `Dropped_Course`.
- Problem type: Binary Classification.

The original datasets are not included in this public repository.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

- Statistical analysis and data visualization.
- Target variable distribution analysis.
- Correlation analysis.
- Identification of customer behavior and cancellation patterns.
- Detection of missing values and outliers.

### 2. Data Preprocessing

- Missing value handling.
- Data cleaning and standardization.
- Outlier detection and treatment.
- Categorical feature encoding.
- Numerical feature scaling.

### 3. Feature Engineering

- Creation of new predictive features.
- Transformation of existing variables.
- Identification of relevant customer and registration characteristics.
- Preparation of data for machine learning models.

### 4. Machine Learning Models

Three classification algorithms were implemented and evaluated:

- Logistic Regression
- Random Forest
- XGBoost

Model development and optimization included:

- Cross-Validation
- RandomizedSearchCV
- GridSearchCV
- Hyperparameter Tuning
- Overfitting Prevention
- Model Comparison

## Model Performance

ROC-AUC was selected as the primary evaluation metric to assess the models' ability to distinguish between cancelled and non-cancelled course registrations.

The final selected XGBoost model achieved a cross-validation ROC-AUC score of **0.9302**.

Model selection focused on predictive performance, stability, and generalization.

Additional evaluation methods included:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Model Explainability

Feature importance and SHAP (SHapley Additive exPlanations) were used to interpret model predictions and identify the key factors associated with course cancellation risk.

## Business Value

The predictive model can support proactive customer retention by identifying high-risk registrations before cancellations occur.

Potential business applications include:

- Personalized customer communication.
- Targeted retention campaigns.
- Identification of high-risk customer segments.
- Improved customer experience.
- Better operational and financial planning.

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

| File | Description |
| --- | --- |
| `README.md` | Project documentation |
| `course_cancellation_prediction.ipynb` | Data analysis and machine learning implementation |
| `requirements.txt` | Required Python libraries |
| `.gitignore` | Git configuration |

## Data Availability

The original training and test datasets are not publicly distributed as part of this repository.

The repository is intended to demonstrate the project's methodology, machine learning implementation, analytical approach, and model performance.

Access to the original datasets is required to reproduce the model training and predictions.

## Authors

Developed collaboratively by Gal and Aviv as part of an academic Machine Learning project at Tel Aviv University.
