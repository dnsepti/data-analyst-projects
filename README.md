# Data Description

We have three DataFrames as follows:  

1. Table *`visits`* (server logs/records containing website visit data):
    * *`Uid`* — user ID
    * *`Device`* — user device
    * *`Start Ts`* — session start date and time
    * *`End Ts`* — session end date and time
    * *`Source Id`* — the advertising source ID, the source by which the user came to the website


2. All dates in this table use the YYYY-MM-DD format..

    Table *`orders`* (data related to orders):

    * *`Uid`* — user ID who created the order
    * *`Buy Ts`* — the date and time the order was made
    * *`Revenue`* — Y.Afisha's income from the order


3. Table *`costs`* (data related to marketing spend):
    * *`source_id`* — Ad source ID
    * *`dt`* — date
    * *`costs`* — expenses for advertising sources on that date

# Purposes
This is the company where we will analyze data on visits to the Y.Afisha website from January 2017 to December 2018, sales data, and marketing cost statistics. From these data, we will help optimize the marketing budget, based on an analysis of related metrics. The end goal is to be able to tell marketing specialists how much money to invest and where to invest it.

# Libraries
*pandas, numpy, matplotlib, scipy, seaborn* 
