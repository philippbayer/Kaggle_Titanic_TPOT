# Kaggle Titanic TPOT
In this notebook I'm trying to get better scores in Titanic by using TPOT, a new thing that automatically creates machine learning pipelines, see https://github.com/rhiever/tpot

It currently (2017 Feb 12) gets an accuracy of 0.789, not very good. That's not due to TPOT but more due to:

a) sloppy imputation
b) some missing feature extraction (I am ignoring Cabin and Ticket, etc)
c) ???

# TODO:
- come up with better imputation - it should, for example, be possible to predict the missing classes based on Fare and Title (use regression?)
- add more features (currently completely ignoring/dropping Ticket and Cabin)

Based on the leaderboard it should be possible to get to around 0.9. (I believe that the people with accuracy=1.0 are just parsing the names from the publicly available list of survivors)
