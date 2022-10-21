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
The LGBM model performed the best, with Logistic Regression coming as the best non boosting model. Hyperparameter tuning and feature engineering were applied to these two models in an attempt to improve their performance.


## Results

On the test set, the LGBM boosting model performed best with 89% accuracy. After hyperparameter tuning and feature engineering the accuracy actually decreases slightly.


## Recommendations:

I would choose the default LGBM boosting model for production as it performs the best in terms of accuracy, precision, recall, and AUC.


## Limitations & Next Steps

At 918 records, the dataset is on the small side. If additional data can be obtained or appended perhaps the accuracy metric could be improved further.


### For further information

For any additional questions, please contact Richard Shimada at r.shimada@gmail.com.
