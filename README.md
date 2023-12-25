# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import panda

### Step2
<br>
import linear mode; from sklearn

### Step3
Read the file cars.csv

### Step4
Assign the values for x and y as required

### Step5
Create the linearRegression model and predict the output

## Program:
```
#Developed by :-prem.R
#Register number:- 23002486
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)







```
## Output:
![Screenshot 2023-12-25 094235](https://github.com/PREM3112/Multivariate-Linear-Regression/assets/145449383/2f34f8c7-25ab-4124-b24d-60f78ff18945)




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
