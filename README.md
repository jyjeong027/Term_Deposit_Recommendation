# Customer Targeting Strategy for Bank Term Deposit Promotions – Classification Model

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
   - Model evaluation using (Accuracy, Precision, Recall, F1-score):
     - Precision prioritized to keep low false positive which may result in waste of budget
   - Feature Importance Identification
     
3. **Final Outcome**
   - Identify customer characteristics that are most commonly associated with a higher likelihood of subscription

## Conclusion
Based on these results, Bank A can high priority customers can be defined as customers who 
- Responded positively to previous campaigns
- Have a mobile contact method
- Are aged under 20 or over 60
- Have a yearly account balance of at least 2,000
  
**Bank A should send personalized mobile campaigns to this priority customers, as they represent the highest likelihood of term deposit subscription.** 

Addtional strategies include: 
Age-Based Campaign Messaging
- Younger Customers (teens to 20s): Promote term deposits as smart savings for young professionals beginning their financial journey.
- Older Customers (60+): Tailor messages focusing on retirement planning and long-term financial security.

Contact Method Improvement (For Long-Term Gains)
- Encourage customers to update or provide their mobile contact information, since customers reachable via mobile show significantly higher subscription rates.


