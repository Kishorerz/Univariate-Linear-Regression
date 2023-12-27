# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula. ![eqn1](https://github.com/Kishorerz/Univariate-Linear-Regression/assets/144451216/e9a2c5f6-c300-4080-829f-292dc93f3ef1)
4.	Compute the y -intercept of the line by using the formula:  ![eqn2](https://github.com/Kishorerz/Univariate-Linear-Regression/assets/144451216/ac237349-2968-4815-9dd6-bd86ec18827d)
   
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

# Univariate Linear Regression
# Develpoed by: KISHOR KUMAR B.
# Register number: 212223240072
import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
  num+=(x[i]-xmean)*(y[i]-ymean)
  den+=(x[i]-xmean)**2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color="Red")
plt.plot(x,ypred,color="Blue")
plt.show()




```
## Output
</br> ![Screenshot 2023-12-27 210945](https://github.com/Kishorerz/Univariate-Linear-Regression/assets/144451216/0908bb96-3fcb-4112-9e42-911d5e8c732d)
</br>!![Screenshot 2023-12-27 211023](https://github.com/Kishorerz/Univariate-Linear-Regression/assets/144451216/ee94d12f-e7a3-49cb-a353-213c706e5964)

</br>!![Screenshot 2023-12-27 211003](https://github.com/Kishorerz/Univariate-Linear-Regression/assets/144451216/d1aa4b4c-75df-4584-b0c9-c3e83aa09397)

</br>

</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
