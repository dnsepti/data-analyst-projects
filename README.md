# Data Description

The dataset includes the following fields:

- `final_ab_new_users_upd_us.csv` — all users who signed up in the online store from December 7 to 21, 2020
- `final_ab_events_upd_us.csv` — all events of the new users within the period from December 7, 2020 to January 1, 2021
- `final_ab_participants_upd_us.csv` - a table containing the list of experiment participants

Structure of `final_ab_new_users_upd_us.csv`:

- `user_id`
- `first_date` — sign-up date
- `region`
- `device` — device used to sign up

Structure of `final_ab_events_upd_us.csv`:

- `user_id`
- `event_dt` — event date and time
- `event_name` — event type name
- `details` — additional data on the event (for instance, the order total in USD for `purchase` events)

Structure of `final_ab_participants_upd_us.csv`:

- `user_id`
- `ab_test` — test name
- `group` — the test group the user belonged to
    
    
# Purposes
- We have received an analytical task from an international online store. Our predecessor failed to complete it: they launched an A/B test and then quit (to start a watermelon farm in Brazil). They left only the technical specifications and the test results; experiment name is recommender_system_test

- Then, we have to rerun the A/B test to testing changes of the number of events related to the introduction of an improved recommendation system.

# Libraries
*pandas, numpy, matplotlib, seaborn, plotly, scipy, math* 
