# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
STEP1: start

STEP2:Import pandas module and import the required data set.

STEP3:Find the null values and count them.

STEP4:Count number of left values.

STEP5:From sklearn import LabelEncoder to convert string values to numerical values.

STEP6:From sklearn.model_selection import train_test_split.

STEP7:Assign the train dataset and test dataset.

STEP8:From sklearn.tree import DecisionTreeClassifier.

STEP9:Use criteria as entropy.

STEP10:From sklearn import metrics. 10.Find the accuracy of our model and predict the require values.

STEP11: Stop

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Sanjay K
RegisterNumber: 212223220094

import pandas as pd
data=pd.read_csv("C:/Users/admin/Downloads/Employee (1).csv")
data.head()

data.info()

data.isnull().sum()

data['left'].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data['salary']=le.fit_transform(data['salary'])
data.head()

x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','salary']]
x.head()

y=data['left']

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion='entropy')
dt.fit(x_train,y_train)
y_predict=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_predict)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![WhatsApp Image 2024-04-06 at 21 21 00_6994abdd](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/1067967c-ee29-4592-a652-255b8241fe09)

![WhatsApp Image 2024-04-06 at 21 21 14_3f9dd966](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/51f7de6c-6efa-4734-bb3b-9858ce2c5748)

![WhatsApp Image 2024-04-06 at 21 21 33_1fdebb9a](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/05478b98-6db1-45d2-84c4-3adc59a9fc6f)


![WhatsApp Image 2024-04-06 at 21 21 51_7acfe3ad](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/a900c400-401d-4357-a8c0-9902c600d91d)

![WhatsApp Image 2024-04-06 at 21 22 03_b5123fba](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/006a394e-f138-4227-be2a-5901d7dbc454)

![WhatsApp Image 2024-04-06 at 21 22 13_9eba5785](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/c200ec87-64b3-4e9d-ab9b-f6c098bc6d84)

![WhatsApp Image 2024-04-06 at 21 22 22_a8d54a3a](https://github.com/SanjayK2006/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/144979178/00b42803-ae1a-4903-8562-4528de840be0)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
