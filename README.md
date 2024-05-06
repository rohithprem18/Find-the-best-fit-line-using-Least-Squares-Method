# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:
Step-1: Start
<br>Step-2: Get the independent variable X and dependent variable Y.
<br>Step-3: Calculate the mean of the X -values and the mean of the Y -values.
<br>Step-4: Find the slope m of the line of best fit using the formula. <br>
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
<br>Step-5: Compute the y -intercept of the line by using the formula:<br>
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
<br>Step-6: Use the slope m and the y -intercept to form the equation of the line.
<br>Step-7: Obtain the straight line equation Y=mX+b and plot the scatterplot.
<br>Step-8: Stop.
## Program:
```
Program to implement univariate Linear Regression to fit
a straight line using least squares.
Developed by: ROHITH PREM S
RegisterNumber:  212223040172
import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0
```
```
for i in range(len(X)):
    num+=(X[i]-X_mean)*(Y[i]-Y_mean)
    denom+=(X[i]-X_mean)**2
m=num/denom
b=Y_mean-m*X_mean
print(m,b)
y_predicted=m*X+b
print(y_predicted)
plt.scatter(X,Y)
plt.plot(X,y_predicted,color='red')
plt.show()
```
## Output:

![Screenshot (1233)](https://github.com/VARSHINI22009118/Find-the-best-fit-line-using-Least-Squares-Method/assets/119401150/3a23debe-5569-4aad-be5c-adcbb55367f3)

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
