# Executive summary
The study investigates the effectiveness of Deep Learning (DL) in predicting loan defaults for a consumer lending company to improve operations.

Rigorous data preparation techniques were employed to ensure model effectiveness based on a 50,000 observations dataset. We addressed missing values by removing columns with data gaps, created a new column to better categorize regions, applied label encoding to convert ordinal categorical variables and one-hot encoding for nominal categorical variables, and converted date columns into a numerical format.

By implementing and optimizing a 2-layer Dense Neural Network (DNN) model we obtain 96.8% accuracy in predicting bad loans on the test set with 94.6% precision, 84.1% recall and 89% F1-score. Based on these results, limitations, recommendations and further research questions have been discussed.


# Introduction
As a consumer lending company, we are currently facing challenges related to loan approval efficiency, risk assessment, and customer satisfaction. To address these issues, our department is leveraging advanced analytics to improve operational performance and enhance overall business outcomes.

Loan approval, as noted by Abakarim (2018), is a binary classification problem where a set of loan applicants’ data is analyzed and classified as either "good" or "bad" risk. One of the major challenges in lending is identifying applicants who may default on their loans, i.e., those who are unable to repay (Kumar et al., 2018).

Our research aims to address this challenge by applying deep learning (DL) techniques to predict loan defaults. Specifically, we have developed a Deep Neural Network (DNN) model using historical loan data to automate the identification of high-risk applicants. The DNN model is composed of densely connected layers, where each neuron continuously adjusts its weights through learning. These neurons receive inputs from, and transmit outputs to, all neurons in adjacent layers, enabling the model to capture complex patterns within the data (Nazari & Yan, n.d.).

Data preprocessing was a critical step in our workflow, allowing us to cleanse and structure the historical dataset for training and evaluating the DNN model. Our ultimate goal is to create a more efficient, automated solution to loan application approval, reducing risk and enhancing decision-making processes.


# Data
• The loan data contains loans issued through 2012 2013 including the current loan status ( Late, Fully Paid, etc and latest payment information Features (include credit scores, number of finance inquiries, address including zip codes and state, and collections among others. Collections indicates whether the customer has missed one or more payments and the team is trying to recover their money.

• Detailed description is given in the dictionary file The file contains 50 k observations.


# Background
• We are You are working for the analytics department of a consumer lending company.

• The company has been facing challenges related to loan approval efficiency, risk assessments, and customer satisfaction.

• To address these issues, our department has been asked to use advanced analytics to improve their
operations and overall performance.


# Requirement
• Our department seeks to use deep learning on its extensive loan data to predict who will default (“ loan_is_bad ”) in the hopes of building an automated solution to loan applications.

• We need to do some basic feature selection and transformation (i.e. making all values numeric). This may include converting variables to binary or using one hot encoding techniques (etc). However, you will not need to perform the same level of feature engineering you might with a classical approach.

• Use all vali d observations from the loan data (e.g. remove N/A’s etc

• Perform basic feature engineering to ensure data is in a numerical input and any noise variables are removed

• Build a deep learning model, with an appropriate loss function, to predict which customers will default. Use fewer iterations than we did in our first examples

• Validate the results using test data and appropriate metrics and provide recommendations to the company based on our findings.



