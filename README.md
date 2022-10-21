# Predicting heart disease based on various clinical metrics 


**Author**: Richard Shimada

### Business problem:

What biometric factors are most impactful in determining heart disease?

### Data:
Dataset can be found online [here](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction). Some visual callouts on the data set:


![image](https://github.com/Richard-Shimada/Project-2/blob/main/countplots%20of%20various%20biometrics.png)

Supermarkets have the highest total sales volume, with Type 1 stores having the majority of total sales volume (over $12M).


![image](https://user-images.githubusercontent.com/110313483/191889066-f91da510-d333-4c48-9078-c969c13c2100.png)

Within the actual items sold, all item types have a similar MRP in the $130 to $160 range.

## Pre-processing
To prepare the dataset for modeling, I removed duplicates, imputed unknown values, encoded categorial data, and scaled numerical data.


## Modeling

A Linear Regresssion and Regression Tree Model were both fit to the data. The Regression Tree model's max depth was tuned to improve the predictive power of the model.

## Results

On the test set, the linear regression model has an R2 score of 0.57 compared to 0.59 for the regression tree model. 

In addition, mean absolute error, mean squared error, and root mean square error are lower for the regression tree model.



## Recommendations:

Of the two models I would recommend using the regression tree. After tuning, the variance has improved drastically. Furthermore, the error metrics and R2 score are more favorable for the regression tree.


## Limitations & Next Steps

To further improve results, instead of a Linear Regression model we could try a Ridge, Lasso, or Elastic Net model. In addition to the regression tree, we could also try implementing other tree models such as bagged trees and random forests.


### For further information

For any additional questions, please contact Richard Shimada at r.shimada@gmail.com.
