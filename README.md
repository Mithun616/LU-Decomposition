# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Step 1: Import the library numpy as np , from scipy .linalg import lu

2.Step 2: Get the input from the array function

3.Step 3: By using the lu function we can able to find the L U decomposition of a matrix

4.Step 4: End of the program

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
![Screenshot 2024-12-01 143930](https://github.com/user-attachments/assets/ab2aeef1-485f-4b23-a3d5-ef238ccaed63)
![Screenshot 2024-12-01 143948](https://github.com/user-attachments/assets/823e7c6d-52f3-4c1f-8f20-96de1b8f55dc)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

