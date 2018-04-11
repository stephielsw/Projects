## Project Objectives
This project aims to predict whether a restaurant will close or remain in operation based on the business and review data from Yelp dataset. The scope of the project is only limited to restaurants in United States. 

This prediction results will be helpful for evaluating investment decisions on the said restaurant and for bank assessing loan requests from the business.

## Source
The source is from [Yelp open dataset (round 11)](https://www.yelp.com/dataset/download), which contains the below JSON files:
1.	Business – contains location data, business attributes and categories.  The attribute is_open will be used as the target.
2.	Review – contains user reiews
3.	User – contains user data
4.	Checkin – contains checkins on a business
5.	Tip – contains tips written by a user on a business
6.	Photo – contains data on photograph submitted by users on a business

For our project, we will only use Business and Review datafiles.

## Evaluation 
With this classification problem, we will use the Classification Report/Confusion Matrix and ROC as our evaluation metrics.

## Method
We will build and train our models with Logistic Regression, Random Forest, Gradient Boosting, XGBoost and Balanced Bagging Classifier and use cross validation to validate our models' performance.
