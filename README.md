# Project 2: Customer Churn Prediction using Machine Learning 📈

[![Python](https://img.shields.io/badge/Python-3.9+-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/thevivekai/)

This repository contains a comprehensive machine learning project focused on predicting customer churn for a telecommunications company. By analyzing customer data, this project aims to build a reliable classification model that can identify customers who are likely to stop using the company's services. This is a classic and highly valuable business problem, as retaining existing customers is often more cost-effective than acquiring new ones.

## 📜 Table of Contents

  * [Project Objective](https://www.google.com/search?q=%23%F0%9F%8E%AF-project-objective)
  * [Dataset Information](https://www.google.com/search?q=%23%F0%9F%93%8A-dataset-information)
  * [Methodology](https://www.google.com/search?q=%23-methodology)
  * [Exploratory Data Analysis (EDA) Highlights](https://www.google.com/search?q=%23-exploratory-data-analysis-eda-highlights)
  * [Model Performance & Results](https://www.google.com/search?q=%23-model-performance--results)
  * [How to Run This Project](https://www.google.com/search?q=%23-how-to-run-this-project)
  * [File Descriptions](https://www.google.com/search?q=%23-file-descriptions)
  * [Conclusion](https://www.google.com/search?q=%23-conclusion)
  * [Contact](https://www.google.com/search?q=%23-contact)

-----

## 🎯 Project Objective

The primary goal of this project is to develop and evaluate several machine learning models to accurately predict customer churn. The project involves a deep dive into exploratory data analysis (EDA) to uncover insights, followed by rigorous data preprocessing, model training, and performance comparison to identify the most effective algorithm for this task.

-----

## 📊 Dataset Information

The project uses a `Customer_Churn.csv` dataset which contains various attributes of telecommunication customers.

  * **Content:** The dataset includes customer demographics, account information, and services they have signed up for.
  * **Target Variable:** The `Churn` column indicates whether a customer has churned (`Yes`) or not (`No`).
  * **Features:** Include variables like `gender`, `SeniorCitizen`, `tenure`, `MonthlyCharges`, `TotalCharges`, and various service subscriptions (e.g., `PhoneService`, `OnlineSecurity`, `TechSupport`).

-----

## ⚙️ Methodology

The project was executed following a standard data science pipeline:

1.  **Data Loading & Initial Exploration:** The dataset was loaded using Pandas for initial inspection of its structure, data types, and summary statistics.
2.  **Exploratory Data Analysis (EDA):** A thorough EDA was performed to understand the relationships between different features and the target variable (`Churn`). This involved creating visualizations to identify key patterns and correlations.
3.  **Data Preprocessing & Feature Engineering:**
      * Categorical features were converted into a numerical format using One-Hot Encoding.
      * Numerical features were scaled using `StandardScaler` to ensure that all features contribute equally to the model's performance.
4.  **Model Building & Training:** Several classification algorithms were trained on the preprocessed data:
      * Linear Regression
      * Logistic Regression
      * Multiple Logistic Regression
      * Decision Tree Classifier
      * Random Forest Classifier
5.  **Model Evaluation:** Each model's performance was evaluated based on its accuracy score. The best-performing model was then selected for a more in-depth analysis using a classification report and a confusion matrix.

-----

## 💡 Exploratory Data Analysis (EDA) Highlights

The EDA revealed several key insights into the factors influencing customer churn.

  * **Churn Distribution:** The dataset is somewhat imbalanced, with fewer customers having churned.
  * **Contract Type:** Customers with month-to-month contracts are far more likely to churn compared to those with one or two-year contracts.
  * **Online Security & Tech Support:** Customers without Online Security or Tech Support services showed a higher churn rate.
  * **Payment Method:** Customers using electronic check as their payment method had a higher tendency to churn.

-----

## 🏆 Model Performance & Results

The models were evaluated based on their accuracy on the test set. The Gradient Boosting Classifier emerged as the top-performing model.

### Model Accuracy Comparison

| Model | Accuracy Score |
| :--- | :---: |
| Logistic Regression | 74.6% |
| **Multiple Logistic Regression** | **79.7%** |
| Decision Tree Classifier | 76.4% |
| Random Forest Classifier | 76.2% |

### Best Model: Gradient Boosting Classifier

The Multiple Logistic Regression model provided the best balance of precision and recall for predicting churn.

  * **Overall Test Accuracy:** **79.7%**

#### Classification Report

| Class | Precision | Recall | F1-Score |
| :---: | :---: | :---: | :---: |
| **No (0)** | 0.85 | 0.92 | 0.88 |
| **Yes (1)**| 0.69 | 0.54 | 0.60 |

#### Confusion Matrix

The confusion matrix for the Multiple Logistic Regression model shows its effectiveness in correctly identifying both churning and non-churning customers.

-----

## 🚀 How to Run This Project

To run this project on your local machine, follow these steps:

1.  **Clone the Repository:**
    ```bash
    git clone <your-repository-url>
    ```
2.  **Install Dependencies:**
    It's recommended to use a virtual environment.
    ```bash
    pip install pandas scikit-learn numpy matplotlib seaborn
    ```
3.  **Run the Jupyter Notebook:**
    Navigate to the project directory and launch the notebook.
    ```bash
    jupyter notebook P2_ML_Customer_Churn.ipynb
    ```
    You can then run the cells sequentially to reproduce the analysis and results.

-----

## 📁 File Descriptions

  * **`P2_ML_Customer_Churn.ipynb`**: The main Jupyter Notebook containing the complete Python code for data analysis, model training, and evaluation.
  * **`P2_ML_Customer_Churn.html`**: An HTML export of the notebook for easy viewing in any web browser.
  * **`Customer_Churn.csv`**: The dataset used for this project.
  * **`Python Final Project Description.pdf`**: The original project description and requirements document.
  * **`README.md`**: This file, providing a summary of the project.

-----

## ✨ Conclusion

This project successfully demonstrates the application of various machine learning algorithms to predict customer churn. The **Gradient Boosting Classifier** was identified as the most effective model, achieving an accuracy of nearly **82%**. The insights gained from the exploratory data analysis highlight key business areas (like contract types and add-on services) that the telecommunications company could focus on to improve customer retention.

-----

## 📧 Contact

**Vivek Prakash Upreti**

  * **Email:** thevivekai@gmail.com
  * **LinkedIn:** [https://linkedin.com/in/thevivekai](https://linkedin.com/in/thevivekai)
