# credit-risk-classification

The repository will house the requirements for the GWU course assignment, Module 20.

Below are the details of the requirements:


Background In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Before You Begin Create a new repository for this project called credit-risk-classification. Do not add this homework to an existing repository.

Clone the new repository to your computer.

Inside your credit-risk-classification repository, create a folder titled "Credit_Risk."

Inside the "Credit_Risk" folder, add the credit_risk_classification.ipynb and lending_data.csv files found in the "Starter_Code.zip" file.

Push your changes to GitHub.

Files Download the following files to help you get started:

Module 20 Challenge filesLinks to an external site. Instructions The instructions for this Challenge are divided into the following subsections:

Split the Data into Training and Testing Sets

Create a Logistic Regression Model with the Original Data

Write a Credit Risk Analysis Report

Split the Data into Training and Testing Sets Open the starter code notebook and use it to complete the following steps:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

note A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

Split the data into training and testing datasets by using train_test_split.

Create a Logistic Regression Model with the Original Data Use your knowledge of logistic regression to complete the following steps:

Fit a logistic regression model by using the training data (X_train and y_train).

Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluate the model’s performance by doing the following:

Generate a confusion matrix.

Print the classification report.

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

Write a Credit Risk Analysis Report Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

Requirements Split the Data into Training and Testing Sets (30 points) To receive all points, you must:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame. (5 points)

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns. (10 points)

Split the data into training and testing datasets by using train_test_split. (15 points)

Create a Logistic Regression Model (30 points) To receive all points, you must:

Fit a logistic regression model by using the training data (X_train and y_train). (10 points)

Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. (5 points)

Evaluate the model’s performance by doing the following:

Generate a confusion matrix. (5 points)

Generate a classification report. (5 points)

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels? (5 points)

Write a Credit Risk Analysis Report (20 points) To receive all points, you must:

Provide an overview that explains the purpose of this analysis. (5 points)

Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)

Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

Coding Conventions and Formatting (10 points) To receive all points, you must:

Place imports at the top of the file, just after any module comments and docstrings and before module globals and constants. (3 points)

Name functions and variables with lowercase characters, with words separated by underscores. (2 points)

Follow DRY (Don’t Repeat Yourself) principles, creating maintainable and reusable code. (3 points)

Use concise logic and creative engineering where possible. (2 points)

Code Comments (10 points) To receive all points, your code must:

Be well commented with concise, relevant notes that other developers can understand. (10 points)

Overview of the Analysis
In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

Explain the purpose of the analysis.
The goal of this analysis was to develop and evaluate a machine learning model capable of predicting loan status, distinguishing between healthy loans (0) and high-risk loans (1). This helps financial institutions assess loan applications efficiently, minimizing financial risk while maintaining profitability.

Explain what financial information the data was on, and what you needed to predict.
The dataset contains financial information about loan applications, including borrower credit history and financial standing.

Provide basic information about the variables you were trying to predict (e.g., value_counts).
Using value_counts(), the dataset is highly imbalanced

Describe the stages of the machine learning process you went through as part of this analysis.

Data Preprocessing
Model Selection & Training
Model Evaluation
Briefly touch on any methods you used (e.g., LogisticRegression, or any other algorithms).

Logistic Regression was chosen for this analysis because it is a simple yet effective classification algorithm that works well for binary classification problems, such as predicting loan status (healthy vs. high-risk loans)

Results
Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1:

Description of Model 1 Accuracy, Precision, and Recall scores.
• Accuracy Score: 99% • Precision & Recall Scores: • Healthy Loans (0) • Precision: 1.00 → Every predicted healthy loan was correct. • Recall: 0.99 → 99% of actual healthy loans were correctly identified. • High-Risk Loans (1) • Precision: 0.86 → 86% of predicted high-risk loans were actually high-risk. • Recall: 0.94 → 94% of actual high-risk loans were correctly identified.

Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Which one seems to perform best? How do you know it performs best?
• Logistic Regression achieved an overall accuracy of 99%, making it highly effective for predicting loan status

Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the 1's, or predict the 0's? )
Yes, the importance of the model depends on the business objective: • If the goal is to avoid high-risk loans at all costs, then high recall for Class 1 (0.94) makes the model useful. • If the goal is to avoid rejecting too many healthy loans, the precision for Class 1 (0.86) should be improved.

If you do not recommend any of the models, please justify your reasoning.

The Logistic Regression model is recommended, but with adjustments. • The model performs exceptionally well overall, but some false positives (incorrectly flagged high-risk loans) could be reduced.

About
The following repository will be created for the fulfilment of the module 20 challenge for the GW Bootcamp

Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 1 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
Jupyter Notebook
100.0%
Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Stat
