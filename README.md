# classification-challenge

Module 13 Challenge

# Email Spam Detection

## Background
Let's say you work at an Internet Service Provider (ISP) and you've been tasked with improving the email filtering system for its customers. You've been provided with a dataset that contains information about emails, with two possible classifications: spam and not spam. The ISP wants you to take this dataset and develop a supervised machine learning (ML) model that will accurately detect spam emails so it can filter them out of its customers' inboxes.

You will be creating two classification models to fit the provided data, and evaluate which model is more accurate at detecting spam. The models you'll create will be a logistic regression model and a random forest model.

## Instructions
This challenge consists of the following subsections:

1. Split the data into training and testing sets.
2. Scale the features.
3. Create a logistic regression model.
4. Create a random forest model.
5. Evaluate the models.

### Split the Data into Training and Testing Sets
Open the starter code notebook and then use it to complete the following steps.

1. Read the data from [this CSV file](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv) into a Pandas DataFrame.
2. In the appropriate markdown cell, make a prediction as to which model you expect to do better.
3. Create the labels set (y) from the “spam” column, and then create the features (X) DataFrame from the remaining columns.
4. Check the balance of the labels variable (y) by using the `value_counts` function.
5. Split the data into training and testing datasets by using `train_test_split`.

### Scale the Features
1. Create an instance of `StandardScaler`.
2. Fit the `StandardScaler` with the training data.
3. Scale the training and testing features DataFrames using the `transform` function.

### Create a Logistic Regression Model
Employ your knowledge of logistic regression to complete the following steps:

1. Fit a logistic regression model by using the scaled training data (`X_train_scaled` and `y_train`). Set the `random_state` argument to 1.
2. Save the predictions on the testing data labels by using the testing feature data (`X_test_scaled`) and the fitted model.
3. Evaluate the model’s performance by calculating the accuracy score of the model.

### Create a Random Forest Model
Employ your knowledge of the random forest classifier to complete the following steps:

1. Fit a random forest classifier model by using the scaled training data (`X_train_scaled` and `y_train`).
2. Save the predictions on the testing data labels by using the testing feature data (`X_test_scaled`) and the fitted model.
3. Evaluate the model’s performance by calculating the accuracy score of the model.

### Evaluate the Models
In the appropriate markdown cell, answer the following questions:

1. Which model performed better?
2. How does that compare to your prediction?

## References:

- Norman, Ryan, instructor. "UNC AI bootcamp."
- ChatGPT4.