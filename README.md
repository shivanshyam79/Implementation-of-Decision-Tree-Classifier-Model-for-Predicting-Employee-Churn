# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard libraries.

2.Upload the dataset and check for any null values using .isnull() function.

3.Import LabelEncoder and encode the dataset.

4.Import DecisionTreeClassifier from sklearn and apply the model on the dataset.

5.Predict the values of array.

6.Import metrics from sklearn and calculate the accuracy of the model on the dataset.

7.Predict the values of array.

8.Apply to new unknown values.


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: shyam R 
RegisterNumber:  212223040200
import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics   
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```
output:
DATA HEAD
### ![169513081-6f903385-3da1-4ba6-ae1e-27cb76d591a6](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/d706f46e-ff26-4f6e-90ac-89073d102679)
DATA INFO
### ![169513082-47b67344-6c44-4ff8-a520-8c341f312eab](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/a256e26d-3c15-4f3a-a204-bb4972535b31)
dATA ISNULL
### ![169513065-14c88236-9210-487c-a477-78c487c4489a](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/f95f4c0b-1577-4df8-821d-be9211bba536)
DATA ISNULL
### ![169513065-14c88236-9210-487c-a477-78c487c4489a](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/3056baa5-84b0-46ed-baaa-f9450805cac6)
DATA LEFT
### ![169513070-33d9ed74-b4f7-4e46-9966-8c60efbec5e5](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/0a1de218-7437-41d5-b930-a82775439d13)
X HEAD
### ![169513073-402a0256-0d5a-46d6-a34a-271cd223be71](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/54e19292-fc7c-428d-b8a4-7d2525b15b3a)
DATA FIT
### ![169513077-04505194-c763-4523-9d17-fbff648e94dd](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/65da6ff5-7ac1-40d3-942a-1ef52e6fe38d)
ACCURACY
### ![169513079-42266498-9323-4a5a-87d6-94ba3815d40b](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/7c0ce944-8ca0-47fb-a426-fba34db9ffea)
PREDICTED VALUES
###  ![169514059-120bf7f7-e57d-4726-b459-4d9a39cdfd2d](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/ae74053c-329f-45e2-9c4b-e143a50dcb30)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
