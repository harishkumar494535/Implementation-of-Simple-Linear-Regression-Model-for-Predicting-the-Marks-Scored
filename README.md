# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1 Get the independent variable X and dependent variable Y.
2 Calculate the mean of the X -values and the mean of the Y -values.
3 Find the slope m of the line of best fit using the formula:
4 Compute the y -intercept of the line by using the formula:
   
## Program:
```
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])

model = LinearRegression()
model.fit(X, Y)
x_input = float(input("Enter hours studied: "))
predicted_marks = model.predict([[x_input]])
print("Predicted Marks:", predicted_marks[0])

Y_pred = model.predict(X)
plt.scatter(X, Y, label="Actual Data")
plt.plot(X, Y_pred, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression (Using sklearn)")
plt.legend()
plt.show()
'''
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: harish Kumar. G
Register Number: 212225080017 
*/
```

## Output:
<img width="990" height="745" alt="Screenshot 2026-08-25 184112" src="https://github.com/user-attachments/assets/2d0a25f1-a34a-4aed-b986-1604088d93e9" />

## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
