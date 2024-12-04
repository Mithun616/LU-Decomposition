# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix
Step 1:Accept a square matrix as input using eval(input()) and convert it to a NumPy array.

Step 2:Use scipy.linalg.lu to compute P,L and U

Step 3:Store and print the lower triangular matrix L

Step 4: Store and print the upper triangular matrix U

Step 5 :End of the program

(ii) To find the LU Decomposition of a matrix

Step 1:Accept a square matrix A and vector b as inputs and convert them to NumPy arrays using eval(input())

Step 2:Use scipy.linalg.lu_factor to compute the LU decomposition of A and returning lu and piv

Step 3:Use scipy.linalg.lu_solve with the factorized lu and piv, and the vector  b to compute the solution vector X.

Step 4: Print the solution vector X

Step 5: End of the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: MITHUN KUMAR G
RegisterNumber: 24900789 
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: MITHUN KUMAR G
RegisterNumber: 24900789
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
(i) To find the L and U matrix
![Screenshot 2024-12-01 143930](https://github.com/user-attachments/assets/ab2aeef1-485f-4b23-a3d5-ef238ccaed63)
(ii) To find the LU Decomposition of a matrix
![Screenshot 2024-12-01 143948](https://github.com/user-attachments/assets/823e7c6d-52f3-4c1f-8f20-96de1b8f55dc)
## Result:
Thus the program to find the L and U and LU Decomposition of a matrix is written and verified using python programming.

