# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Read the csv file

### Step2
Get the value of X and Y variable 

### Step3
Create linear regression model and fit

### Step4
Predict the CO2 emission of the car where the weight is 2300kg, and the volume is 1300cm cube.

### Step5
print predict output

## Program:
```
##Developed by : shakthi vel v
##REgister No : 24901278
import pandas as pd
from sklearn import linear_model
data= pd.read_csv("cars.csv")

X=data[['Weight','Volume']]
Y=data['CO2']

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)

predictCO2=regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding weight and volume",predictCO2)

```
## Output:

![image 1](<WhatsApp Image 2024-12-29 at 12.19.58.jpeg>)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.