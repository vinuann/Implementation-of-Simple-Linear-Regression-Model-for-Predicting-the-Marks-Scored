# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Start the program and store the input data 2.Find the average of the given values 3.Calculate the slope using the data and averages 4.Find the equation of the straight line 5.Draw the graph and display the result

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Vinuthaa NN
RegisterNumber: 212224040362 
*/
```
PROGRAM
```


import matplotlib.pyplot as plt

X = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
Y = [18, 28, 35, 45, 52, 60, 68, 74, 79, 85, 90, 94]

n = len(X)

mean_x = sum(X) / n
mean_y = sum(Y) / n

num = 0
den = 0
for i in range(n):
    num += (X[i] - mean_x) * (Y[i] - mean_y)
    den += (X[i] - mean_x) ** 2

m = num / den
b = mean_y - m * mean_x

print(f"Y = {m:.2f}X + {b:.2f}")

y_pred = [m * x + b for x in X]

plt.scatter(X, Y)
plt.plot(X, y_pred)
plt.xlabel("Study Hours")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression with Realistic Data")
plt.show()
```


## Output:
<img width="711" height="570" alt="image" src="https://github.com/user-attachments/assets/67204828-59bd-42cc-8861-8c979a862081" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
