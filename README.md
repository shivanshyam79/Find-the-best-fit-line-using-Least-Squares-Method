# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
## step 1. Get the independent variable X and dependent variable Y.
## step 2. Calculate the mean of the X -values and the mean of the Y -values.
## step 3. Find the slope m of the line of best fit using the formula. 
## <img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
## step 4. Compute the y -intercept of the line by using the formula:
## <img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
## step 5. Use the slope m and the y -intercept to form the equation of the line.
## step 6. Obtain the straight line equation Y=mX+b and plot the scatterplot.
## step 7 stop
## Program:
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: SHYAM R
RegisterNumber: 212223040200 
*/
```
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
denom=0
for i in range (len(x)):
 num+=(x[i]-x_mean)*(y[i]-y_mean)
 denom+=(x[i]-x_mean)**2

m=num/denom
b=y_mean-m*x_mean
print(m,b)
y_pred=m*x+b
print(y_pred)
plt.scatter(x,y)
plt.plot(x,y_pred,color='red')
plt.show()
```
## Output:
![306845919-bd38b0eb-2b9f-4699-b36b-ce686c63e650](https://github.com/shivanshyam79/Find-the-best-fit-line-using-Least-Squares-Method/assets/151513860/6e98fba4-4a4c-4d21-a826-1171bc49e735)
![306845982-f355297e-3c8f-4988-aa6c-0d103f78ccdc](https://github.com/shivanshyam79/Find-the-best-fit-line-using-Least-Squares-Method/assets/151513860/e3749689-5a34-400c-86af-e8e4b4bdfcb5)




## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
