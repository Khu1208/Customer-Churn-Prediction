# Customer-Churn-Prediction
Customer behaviour using related features and visualizing relation.

## Overview
This repository contains code and resources for predicting customer churn in a telecommunications company using machine learning. Customer churn is a critical metric for businesses to understand because it directly affects revenue. The goal of this project is to develop models that classify customers into different categories (young_solo, young_family, senior_solo, senior_family) and predict churn rates for each category.

## Dataset
The dataset used for this project is [WA_Fn-UseC_-Telco-Customer-Churn.csv](https://www.kaggle.com/datasets/blastchar/telco-customer-churn?resource=download), which contains information about customers of a telecom company, including demographic information, services subscribed, and churn status.

### Features
- `customerID`: Unique identifier for each customer
- `gender`: Customer's gender (male/female)
- `SeniorCitizen`: Whether the customer is a senior citizen (1/0)
- `Partner`: Whether the customer has a partner (Yes/No)
- `Dependents`: Whether the customer has dependents (Yes/No)
- `tenure`: Number of months the customer has stayed with the company
- `MonthlyCharges`: Amount charged to the customer monthly
- `TotalCharges`: Total amount charged to the customer
- `Churn`: Whether the customer churned or not (Yes/No)

## Project Structure
The project is structured as follows:

- `data/`: Folder containing the dataset and any related data files.
- `notebooks/`: Jupyter notebooks for different stages of the project.
  - `1_EDA.ipynb`: Exploratory Data Analysis notebook.
  - `2_Modeling.ipynb`: Modeling notebook for classifying customers and predicting churn.
- `README.md`: This file, providing an overview of the project, dataset, project structure, and findings.

## Exploratory Data Analysis (EDA)
The first notebook, `1_EDA.ipynb`, explores the dataset to understand the distribution of variables, check for missing values, and visualize relationships between features and churn. Key insights include:

- Distribution of gender, seniority, partner status, and dependent status among customers.
- Summary statistics of numerical features (`tenure`, `MonthlyCharges`, `TotalCharges`).
- Correlation between features using heatmap visualization.
- Frequency of churn across different categorical features (`PaymentMethod`, `Partner`, `TechSupport`, `Contract`).

## Modeling
The modeling notebook, `2_Modeling.ipynb`, focuses on building and evaluating machine learning models to classify customers into four categories (`young_solo`, `young_family`, `senior_solo`, `senior_family`) and predict churn rates for each category. Techniques include:

- Data preprocessing and feature engineering to prepare the dataset for modeling.
- Training and evaluating models such as Random Forest, Linear SVC, and SVC.
- Predicting churn rates and compiling results into a summary table.

## Results and Insights
Key findings from the project include:

- Identification of significant predictors of customer churn within different demographic categories.
- Performance comparison of machine learning models for customer classification and churn prediction.
- Insights into customer behavior and recommendations for reducing churn rates.

## Future Work
- Deployment of the best model for real-time predictions.
- Monitoring model performance and updating with new data.
- Exploring additional features or data sources for improving prediction accuracy.

## Requirements
- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, jupyter

Install required libraries using `pip install -r requirements.txt`.

## Author
Your Name (@Khu1208)

Feel free to customize this `README.md` template further based on your specific project details, findings, and insights. This structured approach will effectively showcase your project on GitHub, detailing both EDA insights and modeling results for customer churn prediction.

