# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Input and Initialization
2. Input coefficients and gaussian elimination
3. back substitution
4. output result is given

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: GAYATHRI.K
RegisterNumber: 23013439
import numpy as np
n=int(input())
arr=np.zeros((n,n+1))
res=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        arr[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=arr[j][i]/arr[i][i]
        for k in range(n+1):
            arr[j][k]=arr[j][k]-ratio*arr[i][k]
res[n-1]=arr[n-1][n]/arr[n-1][n-1]
for i in range(n-1,-1,-1):
    res[i]=arr[i][n]
    for j in range(i+1,n):
        res[i]=res[i]-arr[i][j]*res[j]
    res[i]=res[i]/arr[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,res[i]),end=" ")
    

        
*/
```

## Output:
![Screenshot 2023-12-25 103340](https://github.com/GAYATHRI-K06/Gaussian/assets/145742742/2df706fb-c2a5-4ed0-b08a-93edc7cf6266)


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

