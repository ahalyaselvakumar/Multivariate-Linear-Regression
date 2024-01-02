# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
Import pandas as pd.


### Step2:
Read the csv file


### Step3:
Get the value of X and y variables.


### Step4:
Create the linear regression model and fit.


### Step5:
Predict the CO2 emission of a car where the weight is 1000kg, and the volume is 1390cm3.

## Program:
```
#Developed by: AHALYA S
#Reg No: 23002896

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept",regr.predict([[3300,1300]]))

```
## Output:
![OUTPUT](<Screenshot 2024-01-02 195839-1.png>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.