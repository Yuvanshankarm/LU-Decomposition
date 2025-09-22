# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:  
Import required libraries `numpy` and `scipy.linalg`.  

### Step 2:  
Input the matrix/matrices using `eval(input())`.  

### Step 3:  
Perform LU decomposition using `lu()` or solve equations using `lu_factor()` and `lu_solve()`.  

### Step 4:  
Print the results `L` and `U` matrices or solution `X` matrix.

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: Yuvan shankar M
RegisterNumber: 212224220126
'''
import numpy as np
from scipy.linalg import lu
matrix= eval(input())
P,L,U= lu (matrix)
print(L)
print(U)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: Yuvan shankar M
RegisterNumber: 212224220126
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input())) 
lu, pivot = lu_factor(A)
result = lu_solve((lu,pivot),B)
print(result)
*/
```

## Output:
<img width="1882" height="1042" alt="Screenshot 2025-09-22 143840" src="https://github.com/user-attachments/assets/4fcd19fb-2879-4ded-bfde-6e26b98b4972" />


<img width="1916" height="1047" alt="Screenshot 2025-09-22 143859" src="https://github.com/user-attachments/assets/888e9d44-4901-4c43-8255-450516fb4d48" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

