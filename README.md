# HR Employee Retention Prediction

## Project Overview

This project focuses on predicting employee attrition at Salifort Motors using a variety of machine learning models. The goal is to identify which factors contribute to employee turnover and provide actionable recommendations to improve retention.

## Dataset

The dataset used in this project is from the Google Advanced Data Analytics course on Coursera. It includes 14,999 rows and 10 columns, with features related to employee satisfaction, performance reviews, project involvement, and more.

### Features
- `satisfaction_level`: Employee-reported job satisfaction level [0–1]
- `last_evaluation`: Score of employee's last performance review [0–1]
- `number_project`: Number of projects employee contributes to
- `average_monthly_hours`: Average number of hours employee worked per month
- `time_spend_company`: How long the employee has been with the company (years)
- `Work_accident`: Whether or not the employee experienced an accident while at work
- `left`: Whether or not the employee left the company
- `promotion_last_5years`: Whether or not the employee was promoted in the last 5 years
- `Department`: The employee's department
- `salary`: The employee's salary (U.S. dollars)

## PACE Stages

This project follows the PACE methodology:

### Plan
- **Understand the Business Context**: The HR department at Salifort Motors seeks to understand factors contributing to employee turnover to improve retention strategies.
- **Data Familiarization**: Explored the dataset to identify key features and prepare it for modeling.

### Analyze
- **Exploratory Data Analysis (EDA)**: Analyzed relationships between variables and visualized data to understand patterns and insights.

### Construct
- **Model Selection and Construction**: Evaluated various models including Logistic Regression, Decision Tree, Random Forest, and XGBoost Classifier. Constructed and validated these models using appropriate techniques.
- **Model Assumptions**: Verified model assumptions to ensure robustness and accuracy.

### Execute
- **Model Interpretation and Evaluation**: Interpreted model performance using metrics such as precision, recall, F1-score, and AUC.
- **Results Summary**:
  - **Logistic Regression**: Precision: 80%, Recall: 83%, F1-score: 80%, Accuracy: 83%
  - **XGBoost Classifier**: AUC: 94.3%, Precision: 90.6%, Recall: 90.4%, F1-score: 90.5%, Accuracy: 96.8%
  - XGBoost modestly outperformed Decision Tree and Random Forest models.
- **Recommendations**:
  - Cap the number of projects assigned to employees.
  - Consider promoting employees who have been with the company for at least four years.
  - Reassess policies around overtime hours and communicate clearly about overtime pay.
  - Conduct discussions to address company work culture.
  - Implement a proportionate reward system for employees based on effort and contribution.

## Next Steps
- **Data Leakage Concerns**: Investigate the impact of excluding features like `last_evaluation` to test model robustness.
- **Further Analysis**: Consider clustering the data using K-means to derive additional insights.

## Installation

To run this project locally, you need to have Python and the following libraries installed:

- `numpy`
- `pandas`
- `scikit-learn`
- `xgboost`
- `matplotlib`
- `seaborn`

You can install the required libraries using pip:

```bash
pip install numpy pandas scikit-learn xgboost matplotlib seaborn
