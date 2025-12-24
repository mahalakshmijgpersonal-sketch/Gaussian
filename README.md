# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Use import numpy
2. Find gaussian elimination
3. Find the solution
 

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by:MAHALAKSHMI J 
RegisterNumber: 25008001
import numpy as np
from decimal import Decimal,ROUND_HALF_UP
n=int(input())
a=np.zeros((n,n+1))
x=np.zeros(n)
for i in range (n):
    for j in range (n+1):
        a[i][j]=float(input())
for i in range (n):
    if a[i][j]==0.0:
        sys.exit("Divide by zero is detected!")
    for j in range (i+1,n):
        ratio=a[j][i]/a[i][i]
        for k in range(n+1):
             a[j][k]=a[j][k]-ratio*a[i][k]
x[n-1]=a[n-1][n]/a[n-1][n-1]
for i in range (n-2,-1,-1):
    x[i]=a[i][n]
    for j in range (i+1,n):
         x[i]=x[i]-a[i][j]*x[j]
    x[i]=x[i]/a[i][i]
for i in range(n):
    print('X%d = %0.2f' %(i,x[i]),end=" ")
*/
```

## Output:
<img width="661" height="837" alt="Screenshot 2025-12-24 082913" src="https://github.com/user-attachments/assets/e0d704a0-1706-4acd-9627-75e10a900f53" />


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

