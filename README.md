# Data Description

We have three DataFrames as follows:  

The data used in the first part of the project:

1. *`/datasets/hypotheses_us.csv`*
    * *`Hypotheses`* — brief description of the hypothesis
    * *`Reach`* — user reach, on a scale of one to ten
    * *`Impact`* — impact on users, on a scale of one to ten
    * *`Confidence`* — belief in the hypothesis, on a scale of one to ten
    * *`Effort`* — the resources needed to test the hypothesis, on a scale of one to ten. The higher the value of *`Effort`*, the more resource intensive the test is.


Data used in the second part of the project:
    
2. *`/datasets/orders_us.csv`*
    * *`transactionId`* — Order ID
    * *`visitorId`* — ID of the user who made the order
    * *`date`* — the date the order was created
    * *`revenue`* — revenue from orders
    * *`group`* — the A/B test group the user belongs to


3. *`/datasets/visits_us.csv`*
    * *`date`* — date
    * *`group`* — A/B test group
    * *`visits`* — the number of visits on the specified date for the specified A/B test cohort

# Purposes
We are an analyst in a large online store. Together with marketing team, we have compiled a list of hypotheses to help increase revenue. We need to prioritize those hypotheses, run A/B testing, and analyze the results.

# Libraries
*pandas, numpy, matplotlib, scipy, seaborn, warnings* 
