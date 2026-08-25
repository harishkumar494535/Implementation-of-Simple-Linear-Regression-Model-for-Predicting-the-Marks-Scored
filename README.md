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
```import numpy as np
import matplotlib.pyplot as plt

X = np.array([1, 2, 3, 4, 5])
Y = np.array([2, 4, 5, 4, 5])

x_mean = np.mean(X)
y_mean = np.mean(Y)


numerator = np.sum((X - x_mean) * (Y - y_mean))
denominator = np.sum((X - x_mean) ** 2)

m = numerator/denominator
b = y_mean - m * x_mean

print("Slope (m):", m)
print("Intercept (b):", b)

Y_pred = m * X + b
print("Value:", Y_pred)

x = input("Enter value: ")
yy = m * float(x) + b
print("Value:", yy)


plt.scatter(X, Y, label="Data Points")
plt.plot(X, Y_pred, label="Best Fit Line")
plt.xlabel("X")
plt.ylabel("Y")
plt.legend()
plt.title("Univariate Linear Regression")
plt.show()'''
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: harishkumar.G
RegisterNumber: 212225080017 
*/
```

## Output:
<img width="965" height="825" alt="image" src="https://github.com/user-attachments/assets/452d0bbc-8296-450a-acd0-c5b0db7f1fc6" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
