# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import panda as pd.

### Step2
Import linear model from sk learn.

### Step3
Read the csv file.

### Step4
Find the multivariate regression.

### Step5
Dislplay the output.

## Program:
```
# Implementation of Multivariate Linear Regression
# Developed by : PRADEEP E
# Register number : 212223230149
import pandas as pd 
from sklearn import linear_model
data=pd.read_csv("Cars .csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)

```
## Output:

### Insert your output
![ex 10](https://github.com/pradeeprajeswari/Multivariate-Linear-Regression/assets/145743112/d86dd24b-3549-4576-a9dc-54b4474156f2)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
