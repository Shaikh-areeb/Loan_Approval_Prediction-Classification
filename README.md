# Loan Approval Prediction Classification
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/prediction_app_files/personal%20loan.jpg)

This project is a comprehensive Loan Approval Prediction System built using machine learning techniques. 
The system predicts whether a loan application will be approved or rejected based on applicant details. Below are the steps undertaken to develop the model and deploy it as a user-friendly application.

## Table of Contents

- [Objective](#objective)
- [Technologies Used](#technologies-used)
- [Steps in Model Development](#steps-in-model-development)
  - [Step 1: Fetching Data](#step-1-fetching-data)
  - [Step 2: Descriptive Statistics](#step-2-descriptive-statistics)
  - [Step 3: Data Cleaning](#step-3-data-cleaning)
  - [Step 4: Exploratory Data Analysis (EDA)](#step-4-exploratory-data-analysis-eda)
  - [Step 5: Outlier Removal](#step-5-outlier-removal)
  - [Step 6: Label Encoding](#step-6-label-encoding)
  - [Step 7: Addressing Imbalance with SMOTE](#step-7-addressing-imbalance-with-smote)
  - [Step 8: Model Building and Tuning](#step-8-model-building-and-tuning)
  - [Step 9: Model Serialization](#step-9-model-serialization)
  - [Step 10: Deployment with Streamlit](#step-10-deployment-with-streamlit)
- [Key Features](#key-features)
- [How to Use the Application](#how-to-use-the-application)
- [Conclusion](#conclusion)


## Objective

To create a machine learning system that automates loan approval predictions for financial institutions. 
The model identifies patterns in applicant data to ensure fair, efficient, and accurate decision-making.

## Technologies Used

* Python: Data preprocessing, model development, and deployment

* MySQL: Data storage and retrieval

* Scikit-learn: Machine learning and model evaluation

* Streamlit: Web application for user interaction

* SMOTE: Synthetic data generation for addressing class imbalance

* Pickle: Model serialization for deployment

## Steps in Model Development

Step 1: Fetching Data

* Data was retrieved directly from a MySQL database containing loan application records.

Step 2: Descriptive Statistics

* Performed summary statistics to understand data distributions and identify key patterns.

Step 3: Data Cleaning

* Missing Values: Filled missing values using:

* Median for numerical columns

* Mode for categorical columns

* Duplicates: Checked for and removed fully duplicated rows to ensure data consistency.

Step 4: Exploratory Data Analysis (EDA)

* Conducted EDA to understand feature relationships:

* Univariate Analysis: Histograms and box plots for individual features

* Bivariate Analysis: Scatter plots and correlation heatmaps

* Multivariate Analysis: Insights into feature interactions affecting loan approval

Step 5: Outlier Removal

* Removed outliers using statistical techniques (e.g., IQR) to improve model robustness.

Step 6: Label Encoding

* Encoded categorical variables into numerical format using Label Encoding, ensuring compatibility with machine learning models.

Step 7: Addressing Imbalance with SMOTE

* Applied Synthetic Minority Oversampling Technique (SMOTE) to handle class imbalance and improve model performance on minority classes.

Step 8: Model Building and Tuning

* Built and evaluated multiple machine learning models, including:

* Logistic Regression
* Random Forest
* KNN
* SVC
* Decision Tree
* XGBoost (Best Performing Model)

* Performed hyperparameter tuning using GridSearchCV for optimal performance.

Step 9: Model Serialization

* Serialized the best-performing model (XGBoost) using Pickle for deployment.

Step 10: Deployment with Streamlit

* Developed a Streamlit-based web application:
* Users can input applicant details.
* The app predicts loan approval status.
* Saves user data and predictions into the database for analysis.

## Models Perfomance

| Model                | Accuracy   |
|----------------------|------------|
| RandomForest         | 86.184211  |
| XGB                  | 86.184211  |
| DecisionTree         | 82.894737  |
| LogisticRegression   | 77.631579  |
| KNN                  | 76.315789  |
| SVC                  | 73.684211  |

