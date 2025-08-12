# Bank Term Deposit Recommendation – Classification Model

## Project Overview
The objective of this analysis is to apply a classification model to identify a group of customers that are most likely to subscribe to a term deposit to support targeted marketing. 

## Background:
Bank A is launching a new term deposit product but has a limited marketing budget. This means push notifications and marketing campaigns can only be sent to a targeted subset of customers.

## Business Objective and Problem Definition :
Identify and prioritize customers who are most likely to subscribe to the term deposit, ensuring efficient use of marketing resources.

**Analytical Question:
What are the strongest factors influencing customer subscriptions? Among these factors, which customer characteristics are most commonly associated with a higher likelihood of subscription?**
- Analyzed using Classification ML Model (Random Forest) with Feature Importance analysis to determine strongest factors and deep dive into top features to profile high potential customers and recommend optimal target group

## Dataset
The dataset contains following historical data from marketing campaign for similar term deposit product in the past:
- **Customer demographics**: age, job, marital status, education, etc.
- **Financial indicators**: balance, loan status, housing loan
- **Campaign-related features**: contact method, number of contacts, previous campaign outcome
- **Target variable**: `y` (Yes/No – whether the customer subscribed as a result marketing campaign)
  
## Methodology
1. **Data Preprocessing**
   - Handling null values, duplicates, and outliers 
   - One Hot Encoding categorical variables
   - Feature scaling

2. **Model Selection & Training**
   - RandomForest Classifier with Hyperparameter tuning
   - Model evaluation using:
   - Accuracy, Precision, Recall, F1-score 
   - Feature Importance Identification
     
3. **Final Outcome**
   - Identify customer characteristics that are most commonly associated with a higher likelihood of subscription
   - A ranked profile of high-potential customer segments based on key predictive characteristics, enabling Bank A to allocate marketing resources effectively and maximize ROI.
