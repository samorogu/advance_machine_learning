## Suppose that you have a credit scoring task, where you have to create a ML model that approximates expert evaluation of an individual's creditworthiness. Which of the following can potentially be a data leakage? Select all that apply.


* Among the features you have a company_id, an identifier of a company where this person works. It turns out that this feature is very important and adding it to the model significantly improves your score. this is a normal feature, the fact that it improves your score just means it's an important feature


* **First half of the data points in the train set has a score of 0, while the second half has scores > 0.** In a real-world escenario, this will not be present


* **An ID of a data point (row) in the train set correlates with target variable.** In a real-world escenario, this will not be present


## What is the most foolproof way to set up a time series competition?


* Make a time based split for train/test and a random split for public/private. this is vulnerable to leaderboard probing


* **Split train, public and private parts of data by time. Remove all features except IDs (e.g. timestamp) from test set so that participants will generate all the features based on past and join them themselves.** you need to remove all features tfrom the test set to guarantee there isn't a data-leakage


* Split train, public and private parts of data by time. Remove time variable from test set, keep the features. it is possible to reverse engineer the time-ordering and exploit future-peeking


## Suppose that you have a binary classification task being evaluated by logloss metric. You know that there are 10000 rows in public chunk of test set and that constant 0.3 prediction gives the public score of 1.01. Mean of target variable in train is 0.44. What is the mean of target variable in public part of test data (up to 4 decimal places)? 0.7712

$$
N_1/N=-L-ln(1-C) / ln C -ln(1/C)
$$
Where N_1/N is the mean target in test,L is the leaderboard score and C is the constant of mean target of the train 


## Suppose that you are solving image classification task. What is the label of this picture? 3