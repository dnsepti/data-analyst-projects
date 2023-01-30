# Data Description
    
File path: *`/datasets/logs_exp_us.csv`*.

Each log entry is a user action or an event.

- *`EventName`* — event name
- *`DeviceIDHash`* — unique user identifier
- *`EventTimestamp`* — event time
- *`ExpId`* — experiment number: 246 and 247 are the control groups, 248 is the test group


# Purposes
To investigate user behavior analysis of the Food Company app with event-based analytical. What we do are:
1. Study the sales funnel.
2. Study the results of the experiment of an A/A/B test. 
    - The users are split into three groups: two control groups get the old fonts and one test group gets the new ones

# Libraries
*pandas, numpy, matplotlib, plotly, scipy, math, seaborn, warnings* 
