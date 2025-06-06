# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>import pandas as pd.


### Step2
<br>Read the csv file.


### Step3
<br>Get the value of X and y variables.


### Step4
<br>Create the linear regression model and fit.


### Step5
<br>Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
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

<br>![{ECD0577F-1C20-408E-81A4-0F9296DF89F8}](https://github.com/user-attachments/assets/6fac0541-ddb8-4041-aec5-90fed54e1be2)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
