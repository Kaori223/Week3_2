# REST_API_for_fraud-detection
A logistic regression model that detects the fraud in online transactions that can be acced with a REST API

## The Trained model 

Logistic regression is one of the most popular machine learning algorithms for binary classification. This is because it is a simple algorithm that performs very well on a wide range of problems.
The logistic regression model takes real-valued inputs and makes a prediction as to the probability of the input belonging to the default class (class 0)

## The Data 
Three models trained to label anonymized credit card transactions as fraudulent or genuine. Dataset from [kaggle](https://www.kaggle.com/sarathchandra/credit-card-fraud-detection-99-accuracy/comments#144915).

## The API acces points
to be able to use the api , you need first install the requirements 
```
pip install flask
```
Then test the application by runing the code : 
```
python api.py
```
the app will be running on local host port 5000 
with the endpoints : 
### /api/v0/verify 
This endpoint get a JSON object in a  post method , that represents the new transaction 
```
 {
 "V1" : -1.3598071336738,
 "V2" : -0.0727811733098497,
 "V3" : 2.53634673796914,
  ...
  ...
  ...
  ...
 "V25" : 0.128539358273528,
 "V26" : -0.189114843888824,
 "V27" : 0.133558376740387,
 "V28" : -0.0210530534538215,
 "Amount" : 149.62
 }
```

