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

## Output:
DATA HEAD
![169513081-6f903385-3da1-4ba6-ae1e-27cb76d591a6](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/d337db6b-34fb-44f8-8753-231f3ce3c12a)
DATA INFO
![169513082-47b67344-6c44-4ff8-a520-8c341f312eab](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/00ae3668-963c-47e0-b0d8-161b37564576)
DATA ISNULL
![169513065-14c88236-9210-487c-a477-78c487c4489a](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/ff667e54-8c39-40bf-b865-e10059ccad44)
DATA LEFT
![169513070-33d9ed74-b4f7-4e46-9966-8c60efbec5e5](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/c362ec4b-2e5d-4431-b410-ff57776c7d61)
X HEAD
![169513073-402a0256-0d5a-46d6-a34a-271cd223be71](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/c03a1c3b-50c8-44e9-910b-a31c3df19fb5)
DATA FIT
![169513077-04505194-c763-4523-9d17-fbff648e94dd](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/1230bd58-9f65-4922-a326-2f0aa212f31e)
ACCURACY
![169513079-42266498-9323-4a5a-87d6-94ba3815d40b](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/aac9fbfb-a8b2-48bc-b715-96da12c67de1)
PREDICTED VALUES
![169514059-120bf7f7-e57d-4726-b459-4d9a39cdfd2d](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/151513860/f1fc14a1-5d25-4261-969e-f9b0e460d0ca)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
