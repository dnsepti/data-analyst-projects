# Data Description
    
We have 5 datasets, as follows:
1. *`/datasets/megaline_calls.csv`*
2. *`/datasets/megaline_internet.csv`*
3. *`/datasets/megaline_messages.csv`*
4. *`/datasets/megaline_plans.csv`*
5. *`/datasets/megaline_users.csv`*


Megaline rounds seconds to minutes and megabytes to gigabytes. For calls , each individual call is rounded up: even if a call lasts only one second, it will count as one minute. For web traffic , each individual web session is not rounded up. However, the total for the month is rounded up. If a user spends 1025 megabytes this month, he will be charged for 2 gigabytes.

Table *`calls`* (call data):
*	*`id`* — Unique web session ID
*	*`call_date`* — call date
*	*`duration`* — call duration (in minutes)
*	*`user_id`* — ID of the user making the call

Table *`internet`* (web session data):
*	*`id`* — Unique web session ID
*	*`mb_used`* — the volume of data consumed during the session (in megabytes)
*	*`session_date`* — web session date
*	*`user_id`* — User ID

Table *`messages`* (data SMS):
*	*`id`* — A unique SMS ID
*	*`message_date`* — the date the SMS was sent
*	*`user_id`* — ID of the user who sent the SMS

Table *`users`* (data pengguna):
*	*`user_id`* — User ID
*	*`first_name`* — the user's first name
*	*`last_name`* — user's last name
*	*`age`* — user's age (years)
*	*`reg_date`* — subscription start date (dd, mm, yy)
*	*`churn_date`* — the date the user stopped using the service (if the value is missing or not present, the service plan was in use when this data was generated)
*	*`city`* — the city where the user lives
*	*`plan`* — the name of the phone plan

Table *`plans`* (phone plan data):
*	*`plan_name`* — the phone's package name
*	*`usd_monthly_fee`* — monthly fee in US dollars
*	*`minutes_included`* — monthly allocation of calling minutes
*	*`messages_included`* — monthly SMS allocation
*	*`mb_per_month_included`* — monthly data volume allocation (in megabytes)
*	*`usd_per_minute`* — price per minute if the package allocation limit has been exceeded (for example, if a package has an allocation of 100 minutes, then usage starting from the 101st minute will be charged)
*	*`usd_per_message`* — price per SMS if the package allocation limit has been exceeded
*	*`usd_per_gb`* — price per extra gigabyte of data if the package allocation limit has been exceeded (1 GB = 1024 megabytes)

# Purposes
We work as an analyst for the telecom operator Megaline. The company offers its clients two prepaid packages, Surf and Ultimate. The advertising department wants to know which prepaid plan generates more revenue to adjust the advertising budget.

We will do an initial analysis of these prepaid packages based on a relatively small sample of clients. We have data on 500 Megaline clients: who they are, where they are from, what type of plan they use, and the number of calls and messages they sent in 2018.

Our tasks are:
1. To analyze client behavior and determine which prepaid plans bring in more income.
2. Test the hypothesis:
  - The average income of users of Ultimate and Surf phone plans is different.
  - The average income of users in the NY-NJ area is different from the income of users from other regions.

# Libraries
*pandas, numpy, matplotlib, scipy, seaborn* 
