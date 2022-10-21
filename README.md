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
The Logistic Regression and Gradient Boosting models performed the best after hyperparameter tuning.  


## Results

On the test set, the Logistic Regresssion and Gradient Boosting model have an accuracy metric of 86% - 87%. After hyperparameter tuning and feature engineering the accuracy increases only slightly.


## Recommendations:

I would choose the Logistic Regression model for production as the final metrics are very similar to the gradient boosting model but it trains much faster so its paramaters can be refined with ease in the future.


## Limitations & Next Steps

At 918 records, the dataset is on the small side. If additional data can be obtained or appended perhaps the accuracy metric could be improved further.


### For further information

For any additional questions, please contact Richard Shimada at r.shimada@gmail.com.
