# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import panda 

### Step2
<br>Import linear model from sklearn 
### Step3
<br>Read the file cars.csv
### Step4
<br>Assign the values for x and y as required
### Step5
<br> Create the linearRegression model and predict the output
## Program:
```
'''
# Developed by: MARXIN LIJO M
# Register no: 23013468
'''

import pandas as pd
from sklearn import linear_model

df = pd.read_csv('employee.csv')

x = df[['Experience', 'Education']]
y = df['Salary']

regr = linear_model.LinearRegression()
regr.fit(x, y)

print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)

new_employee = [[5, 2]]  
predicted_salary = regr.predict(new_employee)

print("Predicted Salary for the corresponding experience and education:", predicted_salary)
```
## Output:
![292745614-e4fb5217-c4a2-4419-98e2-0a988f14dd18](https://github.com/MARXINLIJO/Multivariate-Linear-Regression/assets/145742540/92f22ab2-c017-4c50-bda6-33a6e7bebf33)
![292745583-9b43054a-c7ab-46b3-bd4c-bbc125c235c4](https://github.com/MARXINLIJO/Multivariate-Linear-Regression/assets/145742540/4d0fe543-22b3-4cb4-9bfb-b7096144cf98)
![292745620-e8274234-77ef-4187-ba76-89af5712de7e](https://github.com/MARXINLIJO/Multivariate-Linear-Regression/assets/145742540/d24c1f79-fe99-4d7b-8caf-856caab11bad)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
