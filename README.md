# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the pandas library for data handling and Import linear_model from sklearn for building the regression model.
### Step2 :
 Use pd.read_csv() to read the dataset from the specified file path.Ensure the dataset contains the required columns: Volume, Weight, and CO2.
### Step3 :
 Initialize a linear regression model using linear_model.LinearRegression().Fit the model with the training data (X and Y) using the fit() method.
### Step4 :
Extract the coefficients of the model using model.coef_.Extract the intercept of the model using model.intercept_.
### Step5 :
 Print the coefficients of the model.Print the intercept of the model.Print the predicted CO2 emission for the given input.

## Program:
```python
Developed By: VISHWA V
Ref no :212224110062


import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:

![alt text](<Screenshot 2025-05-22 091019.png>)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.