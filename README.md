# Predicting heart disease based on various clinical metrics 


**Author**: Richard Shimada

### Business problem:

What biometric factors are most impactful in determining heart disease?

### Data:
Dataset can be found online [here](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction). Some visual callouts on the data set:


![image](https://github.com/Richard-Shimada/Project-2/blob/main/boxplot%20of%20biometrics.png)

Biometrics vary widely between healthy people and those with heart disease - namely blood pressure, cholesterol, heart rate, and Oldpeak.


![image](https://github.com/Richard-Shimada/Project-2/blob/main/catplot.png)
![image](https://github.com/Richard-Shimada/Project-2/blob/main/catplot2.png)

From a categorical variable standpoint, ExerciseAngina, Chest pain, and ST_Slope are all useful in predicting heart disease.

## Pre-processing
To prepare the dataset for modeling, I checked for duplicates, imputed unknown values, encoded categorial data, and scaled numerical data.


## Modeling

A number of classification models were tested - KNN, Logistic Regression, Decision tree, XGBoost, LGBM, and Gradient Boosting.
The Logistic Regression and Gradient Boosting models performed very similarly after hyperparameter tuning.  

## Results

On the test set, the linear regression model has an R2 score of 0.57 compared to 0.59 for the regression tree model. 

In addition, mean absolute error, mean squared error, and root mean square error are lower for the regression tree model.



## Recommendations:

Of the two models I would recommend using the regression tree. After tuning, the variance has improved drastically. Furthermore, the error metrics and R2 score are more favorable for the regression tree.


## Limitations & Next Steps

To further improve results, instead of a Linear Regression model we could try a Ridge, Lasso, or Elastic Net model. In addition to the regression tree, we could also try implementing other tree models such as bagged trees and random forests.


### For further information

For any additional questions, please contact Richard Shimada at r.shimada@gmail.com.
