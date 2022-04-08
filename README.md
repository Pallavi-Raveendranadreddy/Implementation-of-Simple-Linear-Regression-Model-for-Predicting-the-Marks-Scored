# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to implement the simple linear regression model for predicting the marks scored.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Use the standard libraries in python for Gradient Design. 
2.Upload the dataset and check any null value using .isnull() function.
3.Declare the default values for linear regression. 
4.Calculate the loss usinng Mean Square Error. 
5.Predict the value of y. 
6.Plot the graph respect to hours and scores using scatter plot function.
## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by:V.Pallavi 
RegisterNumber:212221240059


import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
abi=pd.read_csv('/content/student_scores - student_scores.csv')
abi.head()
X=abi.iloc[:,:-1].values
X
y=abi.iloc[:,1].values
y
from sklearn.model_selection import train_test_split
X_train,X_test,y_train,y_test=train_test_split(X,y,test_size=1/3,random_state=0)
from sklearn.linear_model import LinearRegression
regressor=LinearRegression()
regressor.fit(X_train,y_train)
y_pred=regressor.predict(X_test)
y_pred
y_test
plt.scatter(X_train,y_train,color='red')
plt.plot(X_train,regressor.predict(X_train),color="purple")
plt.title("h vs s (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(X_test,y_test,color='black')
plt.plot(X_test,regressor.predict(X_test),color="orange")
plt.title("h vs s (Testing Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
 
*/
```

## Output:
![simple linear regression model for predicting the marks scored](https://github.com/Pallavi-Raveendranadreddy/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/blob/55364a58c18ac0c47715141961c29c6b879a847a/exp1.PNG)


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
