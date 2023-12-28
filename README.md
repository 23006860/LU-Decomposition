# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. read the elements of augmented matrix into array a and b
2. calculate elements of L and U
3. print L and U matrix
4. find V by solving LV = B by forward substitution
5. find X by solving UX = V by backward substitution
6. print array X as the solution 

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: RAHUL V
RegisterNumber: 23006860
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
p,l,u=lu(A)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: RAHUL V
RegisterNumber: 23006860
'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
![Screenshot 2023-12-28 111532](https://github.com/23006860/LU-Decomposition/assets/139841752/6005d5f9-39b4-465e-bb76-126e534be01a)
![Screenshot 2023-12-28 111556](https://github.com/23006860/LU-Decomposition/assets/139841752/46abf2c1-b625-4b6f-85b8-85b98df75e2f)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

