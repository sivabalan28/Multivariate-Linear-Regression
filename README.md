# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas
### Step2
Read csv file
### Step3
Get data from the csv file
### Step4
Use linearregression and linearfit 
### Step5
Print output
## Program:
```python
#program to implement multivariate linear regression and predict the output
#Developed by:Sivabalan S
#Register number: 2204401
import pandas as pd
from sklearn import linear_model

data=pd.read_csv("cars.csv")

X=data[["Weight","Volume"]]
Y=data["CO2"]

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("coefficients:",regr.coef_)
print("intercept:",regr.intercept_)

predictC=regr.predict([[3300,1300]])
print('predicted C02 for the corresponding weight and volume',predictC)

```
## Output:
![output](outputo1.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
