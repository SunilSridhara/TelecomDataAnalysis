# TelecomDataAnalysis
Analysis of sample Telecom Data
Data file used: https://community.watsonanalytics.com/wp-content/uploads/2015/03/WA_Fn-UseC_-Telco-Customer-Churn.csv?cm_mc_uid=58920755505115141495567&cm_mc_sid_50200000=1514149556&cm_mc_sid_52640000=1514149556
Problem statement:
You are hired as a Product Manager by a Telecom Service provider. You are given the data of all customers. Your job is to ,
 a) If  Telecom provider wanted to give a new 5G plan offer - How will you figure out how many customers should be part of the offer?
 b) Predict which customers are likely to switch to another firm
 c) Show to the executive management a visual chart that shows the segments of the customers that we currently have grouped by certain behavioural elements 
How do you do that?

This problem is solved using clustering algorithm. Since the data is combination of categorical and integer types, Grower distance is used and clustering is done using PAM (partitioning around mediods) algorithm.
PAM is a iterative clustering procedure. In this algorithm
1) First K random data instances or entities is chosen to be mediods
2) Every data instance is assigned to its closest mediods
3) Then for every cluster, new mediod is assigned based on the data instance that would yield lowest average distance if it were re-assigned as mediod.
4) If atleast one mediod is changed then repeat from (b) otherwise algorithm ends.

Data Analysis:
Cluster 1 : Moderates, Cautious in spending, Could be Middle age
Cluster 2 :  Tech savvy, Conservative in spending, Could be Teenagers
Cluster 3 :  Tech savvy, Do not mind spending, Could be Youths, Middle age
Cluster 4 :  Highly Conservatives, Could be Sr. Citizens

Q a) If Telecom Provider wanted to give a new 5G plan offer - How will you figure out how many customers should be part of the offer?
Obvious choice is to offer for Tech savvy and who can afford. 
Choice is Cluster 3.

Q b) Predict which customers are likely to switch to another firm
Mostly likely people who are cost conscious, who do not have multiple lines and have not taken much of advanced features like Device protection, Online security and Tech Support.
Choice is Cluster 1 and Cluster 2 people .

Q c)
 Plots as in the .rmd file.
