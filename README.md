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
