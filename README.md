# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
Import the required libraries such as pandas and LinearRegression from sklearn.

### Step2:
Read the dataset file using pd.read_csv() and store it in a dataframe.

### Step3:
Select the independent variables (Volume and Weight) as x and the dependent variable (CO2) as y.

### Step4:
Create the linear regression model using LinearRegression() and train the model using the fit() method.

### Step5:
Display the coefficient, intercept, and predict the output for the given input values using the predict() method.

## Program:
```
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

<img width="421" height="86" alt="image" src="https://github.com/user-attachments/assets/772c0e3f-71e7-4715-891d-b4ee93035cf1" />

### Insert your output

<img width="421" height="86" alt="image" src="https://github.com/user-attachments/assets/e14b3923-5a6b-4268-bded-01c5b9b76cbe" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
