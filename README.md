# Telco-Customer-Churn
The data set includes information about:

 - Customers who left within the last month – the column is called Churn
 - Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
 - Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
 - Demographic info about customers – gender, age range, and if they have partners and dependents

# Data Source
This dataset contains 7043 rows and 21 columns. Out of 21, there is a column called "Churn" that will be the target variable, while the rest of 20 columns are the predictors and a unique identifier.

Source: https://www.kaggle.com/blastchar/telco-customer-churn

# Objective
The objective of this project is to build predictive modeling of customer churn using an Artificial Neural Network (ANN). If the target variable corresponds to "Churn" is yes, it means this customer has no longer subscribed to this telco company's services.

In this project, we want to minimize the number of False Negative predictions which means we failed to predict the customer that most likely will churn and lost the revenue from them. If we failed to catch a lot of the customer who intends to churn, means the company will lose a big amount of revenue they previously get from those customers which are bad for the company. Thus, the proper metric for the model evaluation is Recall since recall considers the amount of FN that the model can reduce.

In addition to the recall, we also have to evaluate the overall performance of the model. We can use accuracy or area under the curve score. But first, we have to check on the target variable distribution. If the target distribution is imbalanced, we will choose the area under curve as the evaluation metrics.
