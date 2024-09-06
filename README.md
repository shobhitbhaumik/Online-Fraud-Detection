# Online Fraud Detection Project 

### Find Jupyter Notebook With the following link: [Link to Jupyter Notebook](https://github.com/shobhitbhaumik/Online-Fraud_Detection/blob/main/OnlineFraudModel.ipynb)


## Table of Contents
### 1.Overview
### 2. Data Description
### 3. Exploratory Data Analysis
<br><br>

## Overview 
This project deals with data regarding online transactions with features including amount, recipient, nature of transaction and isFraud etc. In this project I will attempt 
to understand the data and build a classification model that will be able to predict whether the transaction is a fraud or not based on various factors.
<br><br>
## Data Description
1. step: Represents a unit of time where 1 step equals 1 hour
2. type: type of online transaction
3. amount: amount of the transaction
4. nameOrg: customer starting the transaction
5. oldbalanceOrg: old balance of the origin customer
6. newbalanceOrg: new balance of the origin customer
7. nameDest: recipient of the transaction
8. oldbalanceDest: old balance of the recipient before the transaction
9. newbalanceDest: new balance of the recipient after the transaction
10. isFraud: Classifies whether the transaction is fraudulent or not


## Exploratory Data Analysis
### Questions
1. What is the distribution of fraudulent cases and legitimate?
2. Who are the top customers by amount?
3. What is the relationship between type of transaction and whether a transaction is a fraud?
4. What is the relationship between amount and step and whether a transaction is a fraud?

   <br><br>
### Findings
##### 1. There is a class imbalance ratio of 917:1 where legimate cases are in significant majority

<img src="https://github.com/user-attachments/assets/471169b4-fe9b-4a6e-98bc-d4c86ef3d07c" width="400" height="300"> <br>


#### 2. The top 10 customers by amount are the following

<img src="https://github.com/user-attachments/assets/671b2802-4d6d-4423-9a79-71fd5092bf87" width="600" height="300">  <br>


#### 3. Cash Out transactions are the most common type followed by Payment.
   However fraudulent transactions are only prevalent in Cash out and Transfer types
   
<img src="https://github.com/user-attachments/assets/f6f8457b-0bbf-40c9-8e04-cbb520619677" width="400" height="300"> <img src="https://github.com/user-attachments/assets/8f8f5502-ae57-4d41-b614-431e730d530a" width="400" height="300" >
<br>

#### 4. Most instances of Fraud Transactions are concentrated from step 50 to 90 and have lower amounts
   <img src="https://github.com/user-attachments/assets/ad2ebde2-2037-4701-b881-a11708efdb87" width="400" height="300">

## Classification Model

### Preparation for Model Building
1. One Hot Encoding for Type columns
2. Splitting data into train and test

### Models Used 
**1. Decision Tree Classifier**
**2. Random Forest Classifier**
**3. XGBoost Classifier (With and Without SMOTE Overssampling)**

### Model Comparison
<img src="https://github.com/user-attachments/assets/56e6528f-18de-4aa7-8101-be45a558a602" width="600" height="400">







   
      
