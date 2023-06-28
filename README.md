# Credit Card Defaulter Prediction

# Overview:
In present day majority of people are using credit card for online shopping, EMI payments. Moreover banks are encouraging customers to use it by approving them freely without any initial charges. Becausecredit card interest income is the major share of profit for all commercial banks. Even if customers are not willing to buy, bank marketing team reaches out through phone call to sell it. At first the interest rate are normal to grope the customer into the practice of using it, later they will levy charges on everything to loot money from the customers. Due to this reason many customers are facing difficulty in repaying the
credit amount on time. If they missed the deadline the interest rate will get multiplied leading to defaulting the account if left unpaid even for a short span of time. The model we are going to build will consider all inputs from user to predict whether the account will be defaulted or not based on various
parameters.

![image](https://github.com/SupriyaSingh1997/ccd/assets/128996364/06346ea7-e5e5-49d7-9f80-6713f4a1eb8b)

## 1. Understanding the Problem Statement: 

The goal of this study is to identify credit card users who are more likely to experience a payment default in the upcoming month. Many organisations that issue credit cards are developing predictive models that will enable them to anticipate a customer's payment status using the customer's credit score, credit history, payment history, and other data. The goal of this research is to estimate the likelihood that a specific client would go into default the following month utilising personal and financial data about the consumer, such as credit line, age, repayment history, and delinquency history for the previous six months. To create a binary predictive model, numerous statistical and data mining approaches will be employed. It will be easier for credit card issuing corporations to pursue specific clients, make strategic efforts to avert defaults, and effectively offset future losses if they are able to accurately identify the impending default of customers in advance. In any case, the material does not explicitly identify any specific person or offer details that could be used to decrypt a connection to a specific person. The goal of this study is to forecast the likelihood that credit card users will become indebted in the following month using payment information from October 2015 to March 2016. Out of the 30,000 observations overall,The binary variable for default payment in April 2016 (Yes = 1, No = 0) must be determined.

## 1.1 Proposed Solution
The proposed model will be capable of studying customers based on various parameters like
gender, education qualification, marital status, previous repayment history and current outstanding
balance. Based on that it can predict the account default status in advance and notify the respective
bank official for further action.


## 2. Data Pre-processing: 

We must carry out fundamental data pre-processing tasks like null value imputation and the removal of undesirable data before moving on to the exploration stage.
### 2.1. Libraries Used 
Pandas ,Numpy , Matplolib, Seaborn,Sklearn

The dataset contains 30000 rows and 25 columns. But we only need information about important columns. and dropping other unwanted columns.

### 2.2. Handling Null Values:
The dataset contains a small number of null values. The majority of the dataset contains null values, which causes several processing bottlenecks. As a result, it is necessary to identify the columns that include lump sum null values and get them discarded. Therefore, let's remove these null values columns that have more than 80% null values.

## 3. PREPARING DATA FOR EXPLORATORY DATA 
ANALYSIS(EDA) 
### 3.1. Data loading
We first put the data onto our drive, and then, using the pandas library, we loaded it into Google Colab Notebook.
### 3.2. Renaming the columns 
This method is useful because it lets you modify a column heading 
without having to create a new column.
### 3.3. Removing unwanted columns from dataset 
### 3.4. Renaming the columns
One way of renaming the columns in a Pandas data frame is by using the rename() function. This method is quite useful when we need to rename some selected columns because we need to specify information only for the columns which are to be renamed.

## 4. EXPLORATORY DATA ANALYSIS 
### 4.1 Shape :
We can find out how many observations and variables we have in the data collection by looking at the shape attribute. It is employed to verify the data's dimension. More than 30000 observations and 23 variables make up the provided data set.  
### 4.2. Describe :
It generates a stats summary for the columns in the DataFrame. The mean, standard deviation, and interquartile range are provided by this function. Additionally, function summarises the numerical columns while excluding the character columns.  

### 4.3. Analysis of different variables
### 4.3.1. Analysing the customers based on their Education 

### 4.3.2. Analysing the age of the customers
### 4.3.3. Analysing the Marital status of the customers

### 4.3.4. Analysing the Gender of the customers

## 5. Training the models 
### 5.1. Fitting different models 
For modeling we tried various classification algorithms like:

  - SVM,
  - Decision Tree
  - Random Forest   
  - Naive Bayes    
  - XGBoost


## 6.  Conclusions
To forecast the client's behaviour in paying off the credit card amount, this project aims to train a variety of supervised learning algorithms. Different resampling strategies were also employed to balance the dataset because in classification issues, an unbalanced dataset is also essential to improving the performance of the model. Using exploratory data analysis approaches, such as data normalisation, we first looked into the datasets. We began with the logistic regression model and then contrasted the findings with models that were based on conventional machine learning.
In the end, the suggested solution was also made available online to help the many parties. Because the decision of whether to pay on time or owing the bill on a particular month usually depends on the prior payment history, the financial institution must look into the client's payment history before considering providing the client a credit card. For instance, a person who has a lot of debt may put off paying the current month's payments unless they receive a windfall that will allow them to pay off all of their debts at once. It is crucial to look at the applicants' credit limits on their active credit cards in addition to their payment history. This is the outcome of a positive feedback loop: Since those who pay their bills on time typically have higher credit scores, banks prefer to extend more credit to them while taking on less risk. Because of this, if a prospective customer already has a credit card with a large credit limit line, they are less likely to default on future payments. When customers apply for credit cards, the financial institution frequently obtains personal data about them, like their age, education level, and marital status; nevertheless, this data also influences the default behavior.
In other words, the financial institution should equally take into account whether to approve a potential customer's credit card or loan application whether they are a man or a woman, have a bachelor's or master's degree, single or married, etc.

We have reached a maximum accuracy of 82% in predicting whether a person will default on their credit card after investigating, altering, and testing several models on the credit card default data set.
Ultimately, it was impossible to determine which model performed the best when attempting to forecast whether or not a person will default on a credit card based just on the accuracy scores of each model. One may observe how closely all these accuracy scores fall in the graph above. In reality, the Random Forest appears to perform the best based just on the accuracy scores.

## 7. References
- Principal Component Analysis, Wikipedia Page, https://en.wikipedia.org/wiki/Principal_component_analysis
- RandomForrestClassifier, http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
- ROC-AUC characteristic, https://en.wikipedia.org/wiki/Receiver_operating_characteristic#Area_under_the_curve
- AdaBoostClassifier, http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html
- CatBoostClassifier, https://tech.yandex.com/catboost/doc/dg/concepts/python-reference_catboostclassifier-docpage/
- XGBoost Python API Reference, http://xgboost.readthedocs.io/en/latest/python/python_api.html





