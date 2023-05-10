# Credit-Card-Fraud-Detection-ML

Author: Maureen Kitang'a

## Problem statement
The problem statement chosen for this project is to predict fraudulent credit card transactions with the help of advanced machine learning models.

In this project, we will analyse customer-level data which has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group.

The dataset is taken from  [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and it has a total of 284,807 transactions, out of which 492 are fraudulent. The dataset is highly imbalanced.

## Business Problem Overview
Retaining high-profit customers is a crucial goal for many banks, but banking fraud poses a significant threat to this objective, causing financial losses and damaging trust and credibility. The global cost of banking fraud is expected to reach $30 billion by 2020, with the increase of digital payment channels resulting in more sophisticated and diverse forms of fraud. Therefore, implementing machine learning-based credit card fraud detection has become a necessity for banks to proactively monitor and prevent fraud, reduce manual reviews, prevent costly fees, and avoid denying legit transactions.

## Defining Fraud
Fraud in the context of credit cards refers to any unlawful activity or behavior aimed at acquiring financial gain by obtaining information without proper authorization from the account holder. One of the most widespread methods of credit card fraud is skimming, which involves duplicating information stored on the magnetic strip of the card. Other forms of credit card fraud include the manipulation or alteration of genuine cards, creation of counterfeit cards, theft or loss of credit cards, and fraudulent telemarketing.

## Data Understanding
The dataset can be downloaded using this [link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.

## Project Workflow
The process can be summarized in the following five steps:

* Data Understanding:we load the data and examine its features to gain insight into the dataset's structure and distribution. This process helps us identify any missing or erroneous data that may need to be addressed before we can proceed with building a model.

* Exploratory data analytics (EDA): we typically perform univariate and bivariate analyses of the data. We also check the correlation between different variables in the dataset.

* Train/Test Split: Now we are familiar with the train/test split, which we can perform in order to check the performance of our models with unseen data. Here, for validation, we can use the k-fold cross-validation method. We need to choose an appropriate k value so that the minority class is correctly represented in the test folds. After this, we scale the sets separately.

* Model-Building: where we select appropriate algorithms and train the model on the prepared dataset. We will then fine-tune the model hyperparameters and predict on both train and test sets.

* Model Evaluation: We need to evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. We need to choose an appropriate evaluation metric which reflects this business goal. In this case , we choose the roc_auc score metric.


For more information or collaboration ; ndungek66@gmail.com
