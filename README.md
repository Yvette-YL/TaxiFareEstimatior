# Taxi Fare Estimatior
A regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered.

## Overview 
The goal of this project was to develop a regression model to estimate taxi fares prior to the ride. The predicted fares will serve as an input for a subsequent machine learning project. This project utilized yellow taxi trip data from New York City collected in 2017.

After analyzing the characteristics of 18 features and their relationships with the target variable (fare amount), six of the most influential features were selected or engineered. A **multiple linear regression model** was then developed, achieving an **R² score of 0.868**, meaning that approximately **86.8% of the variance** in fare amounts is explained by the model, demonstrating strong predictive performance.

## Data Understanding
The dataset, sourced from NYC.gov, contained approximately 408k unique trips with 18 features, including trip duration, pickup and drop-off locationID, vendor information, toll amounts, and payment type, etc. 

Since actual trip distance and duration are unknown before the ride begins, historical trip records were used to calculate the average distance and average duration between pickup and drop-off points.

These averages showed a strong correlation with fare amounts, as illustrated in the heatmap below.
<img alt="Correlation Heatmap" src=/images/heatmap.png>

## Modeling and Evaluation 
Logistic Regression, Decision Tree, and Random Forest models were developed for this project. Among them, the Random Forest model achieved the highest AUC score.
The model identified evaluation score, number of projects, tenure, and overworked as the most important features for predicting employee attrition.
The Random Forest model achieved a precision of 91.51%, recall of 88.76%, F1-score of 90.11%, and accuracy of 96.76%.
<img alt=“Satisfaction-Tenure-Attrition” src=/images/feature-importances.png>
Horizontal bar chart showing feature importance of decision tree and random forest model.

## Conclusion
Excessive workloads combined with insufficient recognition are key drivers of employee attrition.
Retention of long-tenured, high-performing employees is critical to organizational stability.
Implementing effective workload management and formal recognition strategies is recommended to mitigate attrition risks.

---
[My name is Yvette](https://yvette-yl.github.io/ "Welcome to My Profile")  |  [Proposel](/PACE_Strategy.md "")  |  [Python Notebook](/.ipynb "")  |  Presentation  | 
