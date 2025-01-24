### My Streamlit App

Check out my web app here: [My Streamlit App](https://loan-approvalprediction.streamlit.app/)

# Loan Approval Prediction Classification
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/prediction_app_files/personal%20loan.jpg)

This project is a comprehensive Loan Approval Prediction System built using machine learning techniques. 
The system predicts whether a loan application will be approved or rejected based on applicant details. Below are the steps undertaken to develop the model and deploy it as a user-friendly application.

## Table of Contents

- Objective
- Technologies Used
- Steps in Model Development
  - Step 1: Fetching Data
  - Step 2: Descriptive Statistics
  - Step 3: Data Cleaning
  - Step 4: Exploratory Data Analysis (EDA)
  - Step 5: Outlier Removal
  - Step 6: Label Encoding
  - Step 7: Addressing Imbalance with SMOTE
  - Step 8: Model Building and Tuning
  - Step 9: Model Serialization
  - Step 10: Deployment with Streamlit
- Key Features
- How to Use the Application
- Conclusion


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

## Key Features

* Interactive User Interface: Easy-to-use Streamlit app for loan approval predictions.

* Real-time Data Storage: Saves user inputs and predictions into the database.

* Robust Machine Learning Pipeline: Handles missing data, outliers, and class imbalance.

* Optimized Model: Best model selected through rigorous evaluation and hyperparameter tuning.

* Scalable Design: Can handle new data and adapt to changing business requirements.

## How to Use the Application

* Input Applicant Details:
Enter details such as income, education, credit history, and more.

* Submit:
Click on the "Predict Loan Status" button.

* Get Prediction:
The app predicts whether the loan will be approved or rejected.

* Data Storage:
User inputs and predictions are saved to the database for further analysis.

# Conclusion

The XGBoost model was selected as the best-performing model for this project, achieving an accuracy of 86.18%. 
Its superior performance and scalability, XGBoost was the ideal choice for deployment in this loan prediction system.

# Visual Insights Of The Project

## Applicant Income Distribution
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/visual%20insights%20images/Screenshot%202025-01-18%20000509.png)

## Loan Status VS Credit History
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/visual%20insights%20images/Screenshot%202025-01-18%20000550.png)

## Correlation Matrix
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/visual%20insights%20images/Screenshot%202025-01-18%20000133.png)

## Class Imbalaced
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/visual%20insights%20images/Screenshot%202025-01-18%20000153.png)

## Class Balanced Using SMOTE
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/visual%20insights%20images/Screenshot%202025-01-18%20000209.png) 

## Feature Importance
![image](https://github.com/Shaikh-areeb/Loan_Approval_Prediction-Classification/blob/main/visual%20insights%20images/Screenshot%202025-01-18%20000225.png)

## Models Perfomance

| Model                | Accuracy   |
|----------------------|------------|
| RandomForest         | 86.184211  |
| XGB                  | 86.184211  |
| DecisionTree         | 82.894737  |
| LogisticRegression   | 77.631579  |
| KNN                  | 76.315789  |
| SVC                  | 73.684211  |

## Key Objectives of the Loan Approval Prediction Model

- Automate Loan Approval Process:

The model automates the decision-making process, allowing financial institutions to quickly assess loan applications without the need for manual review, saving time and improving operational efficiency.

- Minimize Risk for Lenders:

By predicting the likelihood of loan default based on applicant data, the model helps lenders make informed decisions, reducing the risk of loan defaults and financial loss.

- Improve Decision-Making:

The model enables data-driven decisions, leveraging historical data and applicant features (e.g., credit score, income) to predict loan repayment ability, leading to more accurate and consistent approvals.

- Increase Access to Credit:

By speeding up loan processing and reducing human biases, the model helps more applicants get timely access to credit, benefiting both individuals and businesses.


