# EX 6 Implementation of Decision Tree Classifier Model for Predicting Employee Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula.<p>
![image](https://github.com/user-attachments/assets/0a35246c-911b-49f5-8058-78a4991ede46)

4. Compute the y -intercept of the line by using the formula:<p>
![image](https://github.com/user-attachments/assets/3ac74770-5f52-49f0-bf24-414261e33df4)


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: K.Nishal
RegisterNumber:  2305001021
*/

import numpy as np
import matplotlib.pyplot as plt
x=np.array([2,9,5,5,3,7,1,8,6,2])
y=np.array([69,98,82,77,71,84,55,94,84,64])
XMEAN=np.mean(x)
YMEAN=np.mean(y)
num,den=0,0
for i in range(len(x)):
  num+=(x[i]-XMEAN)*(y[i]-YMEAN)
  den+=(x[i]-XMEAN)**2
m=num/den
c=YMEAN-m*XMEAN
print(m,c)
Y_pred=m*x+c
print(Y_pred)
plt.scatter(x,y)
plt.plot(x,Y_pred,color='red')
plt.show()
```

## Output:
![decision tree classifier model](sam.png)
![image](https://github.com/user-attachments/assets/2a8d6061-25fb-487f-a2ad-d76c5cc5a7ba)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
