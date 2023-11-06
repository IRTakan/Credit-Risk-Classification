# Credit-Risk-Classification

In this Challenge, I used various techniques to train and evaluate a model based on loan risk. 
A dataset of historical lending activity from a peer-to-peer lending services company was used to build a model that can identify the creditworthiness of borrowers.

--This task is divided into the following subsections:--

- Split the Data into Training and Testing Sets.

- Create a Logistic Regression Model with the Original Data.

- Write a Credit Risk Analysis Report.

--Split the Data into Training and Testing Sets-- 

 - I Read the lending_data.csv data from the Resources folder into a Pandas DataFrame. Created the labels set (y) from the “loan_status” column, and then created 
 the features (X) DataFrame from the remaining columns.  Afterwards I split the data into training and testing datasets by using train_test_split.

--Create a Logistic Regression Model with the Original Data--

Used my knowledge of logistic regression to complete the following steps:

- Fit a logistic regression model by using the training data (X_train and y_train).

- Saved the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluated the model’s performance by doing the following:

- Generated a confusion matrix.

- Printed the classification report.

- Answered the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

--Write a Credit Risk Analysis Report--

- Wrote a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework.

Structured my report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

- An overview of the analysis.

- The results: Using a bulleted list, describing the accuracy score, the precision score, and recall score of the machine learning model.

- A summary: Summarized the results from the machine learning model. Included my justification for recommending the model for use by the company.

# Overview of the Analysis

Lending_data.csv was used to build a machine-learning model that evaluates borrowers and identifies their creditworthiness.
These are the factors that were considered in the analysis:

- The size of the loan.
- Interest rate.
- Borrower's Income.
- Debt to income ratio.
- Number of accounts the borrower held.
- Derogatory marks against the borrower.
- Total debt.

The dataset of 77,536 data points was split into training and testing sets. The training set was used to build an initial logistic regression model (Logistic Regression Model 1) using the LogisticRegression module from scikit-learn. Logistic Regression Model 1 was then applied to the testing dataset. The purpose of the model was to determine whether a loan to the borrower in the testing set would be low- or high-risk and results are summarized below.

Two different Logistic Regression models were created by using the original data set and randomy over resampled data set (to get rid of the imbalances). In the end, their results -which was gathered with scikit-learn library- were compared. The resampled data was used to build a new logistic regression model (Logistic Regression Model 2). The purpose of Logistic Regression Model 2 was to determine whether a loan to the borrower in the testing set would be low or high-risk.

--Results--

Logistic Regression Model 1:

- Accuracy: 0.99.
- Precision: For healthy loans the precision is 1.00, for high-risk loans the precision is 0.85.
- Recall: For healthy loans the recall score is 0.99, for high-risk loans the recall score is 0.91.

Logistic Regression Model 2:

- Accuracy: 0.995.
- Precision: For healthy loans the precision is 0.99, for high-risk loans the precision is 0.99.
- Recall: For healthy loans the recall score is 0.99, for high-risk loans the recall score is 0.99.

--Summary--

- Logistic Regression Model 1 which uses original data and does a great job at predicting healthy loans with accuracy, precision and recall close to 100%. However it performs noticably worse at identifying high-risk loans where it has a precision of 85% and a recall of 91%. This tells us that this model is less able to classify high risk loans than healthy loans. This is likely related to the skew in the data that was provided, with only about 3% of the sample being in the high risk loans category. 

- The Logistic Regression Model 2 that uses resampled data, performs noticably better at identifying high risk loans in addition to identifying healthy loans. The overall prediction rate is consistent across precision, recall, and accuracy. I believe its best to utilizie the second model because of its heightened ability to detect high risk loans more accurately. 
This is especially important given how much it can cost a loan provider to misidentify and lend money to a high risk loan applicant, and the minimal cost of misidentifying a healthy loan applicant. One thing that is certain is that model 1 is better at identifying healthy loan applicants, but this is less important than correctly identifying high risk loan applicants, which is accomplished better with model 2.

*Technologies used: Microsoft Visual Studio Code. Languages: Python
