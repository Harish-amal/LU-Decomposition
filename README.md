# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
5a)

Step1:

Import the numpy module to use the built-in functions for calculation

Step2: 


Get lists from input and assign in np.array()

Step3: 

Using the lu(),We can find the solution

Step4: 

print and End the program

5b)

Step1:

Import the numpy module to use the built-in functions for calculation

Step2:

Get lists from input and assign in np.array()

Step3:

Using lu_factor() and lu_solve(),We can find the solutions

Step4:

print and End the program

## Program:
(i) To find the L and U matrix
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu

A=np.array(eval(input()))

p,l,u=lu(A)

print(l)

print(u)

(ii) To find the LU Decomposition of a matrix
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu_factor,lu_solve

a=np.array(eval(input()))

b=np.array(eval(input()))

l,p=lu_factor(a)

x=lu_solve((l,p),b)

print(x)

## Output:
5a)

<img width="1235" height="845" alt="Screenshot 2026-10-15 212407" src="https://github.com/user-attachments/assets/8c647da8-e4cd-4831-a31f-6c0ae6d24737" />

5b)

<img width="1221" height="797" alt="image" src="https://github.com/user-attachments/assets/965f92d6-ae25-4202-9dfd-32d58253c644" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

