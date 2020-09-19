# Customer-Churn

## Business Value

Customer churn is a major problem and one of the most important concerns for companies due to the direct effect on the revenues. Therefore it is important to develop means to predict potential customer to churn. Hence finding factors that increase customer churn is important to take necessary actions to reduce this churn. 

## Problem Statement

To predict customer churn based on various variables like customer account information and customer activity.

## Data

![](Images/Data%20Sample.PNG)

Each row of data represents a customer and each column contains's a customer's attributes.

__Customers who left/churned__ : _Exited_ 

__Demographic Information of customers__ : _Geography_ , _Gender_ , _Age_ 

__Customer Account Information__ :_Tenure , HasCrCard , Balance , IsActiveMember , EstimatedSalary , NumOfProducts , CreditScore_ 

## Approach

+ Loading Data

+ Data Exploration

+ Spliting Data for Train, test and Validation

+ Data Visualization
    - Univariate
    - Bivariate
    
+  Finding Missing Values

+ Label Encoding 

+ One Hot Encoding of Categorical Values
+ Feature Scaling and Normalization

+ Feature Selection

+ Training Model

	- Logistic Regression
	- SVM 
	- Decision Tree

In order to measure the performance of the model, the Area Under Curve (AUC) standard measure, and Accuracy is adopted 

## Visualizing Data

### Data Distribution

__Product Distribution__

![](Images/Products%20Distribution.PNG)

__Salary Distribution__

![](Images/Salary%20Distribution.PNG)

__Tenure Distribution__

![](Images/Tenure%20Distributioin.PNG)

__Balance Distribution__

![](Images/Balance%20Distribution.PNG)

__Customer Age vs Customer Churn__

![](Images/Age%20vs%20Exited.PNG)

__Account Balance vs Customer Churn__

![](Images/Balance%20vs%20Exited.PNG)

__Correlation Heat Map of All Features__

![](Images/HeatMap%20features.PNG)

## Feature Selection

__Selected Features__

![](Images/Selected%20Features.PNG)

## Model Building and Training

1. ### __Logistic Regression__

__Training Data__

![](Images/Logistic%20training%20metrics.PNG)

__Validating Data__

![](Images/Logistic%20validation%20metrics.PNG)

2. ### __SVM Model__

__Training Data__

![](Images/SVM%20Training.PNG)

__Validating Data__

![](Images/SVM%20Validation.PNG)

3. ### __Decision Tree Model__

__Training Data__

![](Images/Decison%20Tree%20Training.PNG)

__Validating Data__

![](Images/Decision%20Tree%20Validation.PNG)

__Comparing All Clasifiers__

![](Images/Classifier_comparison.PNG)

From the Model Comparison we see that Decision Tree Model has better Area Under curve and Accuracy over the other two models.

## __Conclusion__
The precision of the model on previously unseen test data is slightly higher with regard to predicting 1's i.e. those customers that churn. However, in as much as the model has a high accuracy, it still misses some of those who end up churning. The model could be improved by providing and retraining the model with more data over time. :-)
