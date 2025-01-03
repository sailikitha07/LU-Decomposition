# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm for program 1

```

(i)1.Import the numpy library for numerical operations and the scipy.linalg 
   library for 
   linear  algebra functions.
   2. Use the input() function to get a string representation of matrix A 
   from the user,
   and then use eval() to convert it into a numpy array.
   3.Use the lu() function from scipy.linalg to perform LU decomposition on 
   matrix A,which     returns  the permutation matrix P, lower triangular 
   matrix L, and upper triangular matrix U.
   4.Extract the L and U matrices from the LU decomposition result and store
    them in separate variables.
   5.Print the L and U matrices using the print() function.

   ```

## Algorithm for program 2

```

(ii)1. Define the package as scipy.linalg import lu.
    2.Get input from user and print L and U matrix by 'print' .
    3.Define a package as "from scipy.linalg import lu_factor, lu_solve" 
    and create the variable as 'X' include the package in that variable.
    4.print the variable 'X

```

## Program:
(i) To find the L and U matrix

```

Program to find the L and U matrix.
Developed by: sailikitha
RegisterNumber: 24009865
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)


```

(ii) To find the LU Decomposition of a matrix

```

Program to find the LU Decomposition of a matrix.
Developed by: sailikitha
RegisterNumber: 24009865

*/# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
![LU decomposition](<Screenshot 2024-11-18 214117.png>)
![LU decomposition](<Screenshot 2024-11-18 214136.png>)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

