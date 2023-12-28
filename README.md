# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Linear_model from sklearn

### Step2
Read the csv file using pandas library

### Step3
Read the csv file using pandas library

### Step4
Enter the parameters of the linear function

### Step5
Print the parameters of the linear function

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars(1).csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
### Insert your output
![image](https://github.com/syedfayaz3105/Multivariate-Linear-Regression/assets/147144126/5e9bee34-22ef-4ff5-817d-2fe2f1bb1149)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
