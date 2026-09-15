# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

Step1 : import pandas as pd.
Step2 : Read the csv file
Step3 : Get the value of X and y variables
Step4 : Create the linear regression model and fit.
Step5 : Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube

## Program:
```


Developed by : Harini Sree N
Register no : 212225230093
import numpy as np
import matplotlib.pyplot as plt
X= np.array([0,1,2,3,4,5,6,7,8,9])
Y= np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(X,Y)
plt.show()
X_Mean=np.mean(X)
Y_Mean=np.mean(Y)
num=0
den=0
for i in range(len(X)):
    num+=(X[i]-X_Mean)*(Y[i]-Y_Mean)
    den+=(X[i]-X_Mean)**2

m=num/den
b=Y_Mean-(m*X_Mean)
print(f"Slope : {m}\nIntercept : {b}")
Y_Pred=(m*X)+b
print(f"Predicted values are : \n{Y_Pred}")
plt.scatter(X,Y,color='Red')
plt.plot(X,Y_Pred,color='Blue')
plt.show()



```
## Output:

<img width="980" height="391" alt="image" src="https://github.com/user-attachments/assets/983bb9e9-2b6b-4770-a4d6-1c509bf3f4d5" />




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
