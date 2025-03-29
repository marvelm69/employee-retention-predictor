# Employee Attrition Prediction

## Overview
This project aims to develop a predictive model to identify employees who are more likely to quit their jobs. The goal is to help HR teams proactively address issues that lead to employee turnover, thereby reducing costs associated with hiring and retaining talent.

## Problem Statement
Hiring and retaining employees are critical but resource-intensive tasks:

- **Complexity**: Hiring and retaining employees require significant capital, time, and skills.
- **Time Costs**: Small business owners spend 40% of their working hours on non-income-generating tasks like hiring.
- **Financial Costs**: Companies spend 15%-20% of an employee's salary to recruit a new candidate.
- **Revenue Loss**: Onboarding a new employee results in revenue loss of 1%-2.5% due to the time it takes to bring them up to speed.
- **Average Costs**: Hiring a new employee costs an average of $7,645 for companies with 0-500 employees.
- **Time to Fill**: It takes approximately 52 days on average to fill a position.

These statistics highlight the importance of predicting employee attrition to minimize recruitment costs and improve retention strategies.

## Dataset
The dataset used for this project was provided by the HR team at a multinational corporation. It contains extensive information about employees, including:

- **JobInvolvement**: Measures how engaged employees are with their work.
- **Education**: Indicates the level of education of the employees.
- **JobSatisfaction**: Reflects how satisfied employees are with their jobs.
- **PerformanceRating**: Evaluates the performance of employees.
- **RelationshipSatisfaction**: Assesses satisfaction with interpersonal relationships at work.
- **WorkLifeBalance**: Indicates the balance between work and personal life.

### Data Source
The dataset is available on Kaggle: [IBM HR Analytics Employee Attrition & Performance Dataset](https://www.kaggle.com/datasets)

## Objective
The primary objective of this project is to build a predictive model that can accurately classify employees as either likely to quit (Attrition = Yes) or not likely to quit (Attrition = No). This will enable HR teams to take proactive measures to retain valuable employees.

## Methodology
1. **Data Preprocessing**: Cleaning and transforming the dataset for model training.
2. **Exploratory Data Analysis (EDA)**: Understanding data distribution and feature importance.
3. **Feature Engineering**: Selecting relevant features to improve model performance.
4. **Model Selection & Training**: Training different machine learning models.
5. **Evaluation**: Measuring model performance using metrics such as Accuracy, Precision, and Recall.

## Results
The models were evaluated based on Accuracy, Precision, and Recall. Below are the results:

| Model                     | Class | Recall | Precision | Accuracy |
|---------------------------|-------|--------|-----------|----------|
| **Logistic Regression**    | 0     | 0.91   | 0.98      | **0.90** |
|                            | 1     | 0.80   | 0.39      |          |
| **Random Forest**         | 0     | 0.88   | 0.98      | 0.87     |
|                            | 1     | 0.60   | 0.15      |          |
| **Artificial Neural Network** | 0     | 0.90   | 0.90      | 0.83     |
|                            | 1     | 0.40   | 0.39      |          |

From the results:
- **Logistic Regression** achieved the highest accuracy (90%), performing well in classifying non-attrition cases.
- **Random Forest** had a slightly lower accuracy (87%) but struggled with precision in predicting employees who left.
- **Artificial Neural Network (ANN)** performed the worst, with an accuracy of 83% and low recall for predicting attrition.

## Conclusion
- The Logistic Regression model performed the best in predicting employee attrition.
- Further improvements could be made using feature selection, hyperparameter tuning, and ensemble methods.
- Insights from this model can help HR teams create retention strategies and minimize employee turnover.

## Future Work
- Implement more advanced deep learning models.
- Conduct hyperparameter tuning for Random Forest and ANN.
- Explore additional datasets to improve generalizability.
