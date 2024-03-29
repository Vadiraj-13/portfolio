---
title: "Predicting centuries in cricket"
date: 2023-02-16T12:39:00+05:30
draft: false
author: "Vadiraj Adabaddi"
tags:
    - "Machine Learning"
    - "Regression"
    - "Multiple Linear Regression"
    - "Support Vector Regression"
    - "Decision Tree regression"
    - "Random Forest Regression"
image: /images/cricket1.jpg
---

### 🔗 [GitHub](https://github.com/Vadiraj-13/Predicting-centuries-in-cricket/)

How to beat Sachin's record of 100 100s!?

A data cleaning and visualisation was performed on a dataset containing cricketers with most runs in all formats.
Through correlation, useful features were extracted and different types of regression models were trained to accurately predict the number of centuries a batter can score at the end of his career.

Columns \
Player:- Player Name \
Span :- Total time period \
Mat :- Total Matches played by player \
Inns :- Total innings \
NO :- Total Not out \
Runs :- Total runs \
HS :- Highest Run in a innings \
Ave :- Average of batting \
BF :- Total Ball faced \
start year :- Starting Year \ 
end year :- Ending Year \
no of years played :- Experience


Technology used: Pandas, Matplotlib, Seaborn and Scikit-Learn


#### Heatmap

![image](/projects/predicting_centuries/centuries_heat.jpg)


#### Observations through correlations


1. Mat,Inns,Runs, Ave, BF,50,4s have high correlation with 100's

- Therefore, in order to score more centuries all you have to do is play more innings, maintain good average and deal in 4s (6s have a very low correlation!).

2. Filtering the features further - Inn, Ave and 4s


#### Paiplot on filtered dataset

![image](/projects/predicting_centuries/centuries_pair.png)

The filtered dataset was trained with Multiple Linear Regression, Support Vector Regression, Decision Tree Regression and Random forest regression.

The r2 scores are as follows:

| Type of model      | r2 score |
| ----------| ----------- |
| Multiple Linear Regression     | 0.83            |
| Support Vector Regression| 0.46             |
| Decision Tree Regression     |     1         |
| Random forest regression       |     0.93         |


Clearly the decision tree regression model wins!

## Conclusion
In order to beat Sachin's record of 100 100s, one should:
1. Play as many innings as possible
2. Maintain a good average
3. Deal in a lot of fours

and just hope that they can beat 'God's' record!




