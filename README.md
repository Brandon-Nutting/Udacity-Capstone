# Udacity-Capstone
Link To Blog Post: https://medium.com/@brandon.c.nutting/predicting-churn-with-pyspark-5ff408e3f582

# Project Motivation
Everyday an enormous number of users will reduce their subscription status, referred to as 'churn' in many instances. These users who decide to churn will result in companies around the world losing revenue, something no company wants. One example of a company that experiences a lot of churn would be music providers, such as Spotify. As someone who has gone back and forth between paid and free accounts with Spotify I found this problem interesting. 

# Libraries Used 
* pySpark - Used to read in data, clean data, and generate features.
* datetime - Used UDF functions for plotting purposes. 
* matplotlib - Used to plot data during the exploration phase.

# Files In Repository
* mini_sparkify_event_data.json - Data used for my analysis. 
* Spark Analysis.ipynb - Script holding all portions of analysis.

# Results
* Using the following generated fields [Thumbs Up Per Day, Thumbs Down Per Day, Errors Per Day, Help Visits Per Day, Avg Songs Played Until Home, Avg Songs Until Help Needed, Avg Songs Until Error Experienced] I found that the randomForestClassifier returned the best results. Using that model I found that we obtain a perfect 1.0 F1 Score. 
* Since this is a classification problem, I believe we should be most interested the accuracy of the model. That is why I focused on maximizing F1 score.
* I should note, to develop a better model I believe we would need more data. Specifically, we should increase the number of users who actually churned.

# Acknowledgments:
I found the following links very helpful in finishing the project:
* https://stackoverflow.com/questions/58404845/confusion-matrix-to-get-precsion-recall-f1score
* https://stackoverflow.com/questions/28971989/pyspark-mllib-random-forest-feature-importances