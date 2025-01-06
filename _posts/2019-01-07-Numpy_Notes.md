---
title: Numpy Notes
description: Notes on Numpy Library of Python
tags: Python, AI, Machine Learning, Notes
---
**What is NumPy?**  
According to Wikipedia -  
NumPy is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.  

![](https://thepracticaldev.s3.amazonaws.com/i/bhpsnl4f6zv9dz8ejicf.png)
---
**Install NumPy**
a) If you already have Anaconda installed in your PC, then NumPy might be pre-installed in it or simply install it by running -  
`conda install numpy`  
b) If you have pip installed in your PC, then run -  
`python -m pip install — user numpy`  

---
**Import the Library**  
`import numpy as np`  
You can also give other name instead of np.  

---
**Create Arrays and change elements of array**  
a) 1D Array  
`arr1 = np.array([1,2,3,4,5,6])`  
b) Higher Dimension Array  
`arr2 = np.array([[1,2,3],[4,5,6]])`  
c) Change an element of Array  
`arr1[1] = 22` # [1,22,3,4,5,6]  
`arr2[1][1] = 56` # [[1,2,3],[4,56,6]]  
d) Create a matrix/array with all its elements zero  
`arr3 = np.zeros(3)` # creates an array of 3 elements  
`arr4 = np.zeros((2,3))` # creates a matrix of 2 rows and 3 columns  
e) Create an Identity Matrix  
`arr5 = np.eye(4)` #creates a 4X4 identity matrix  
f) Creates a matrix/array with all its elements one  
`arr6 = np.ones((3,4))` # creates an array of 3 rows and 4 columns  
g) Creates a evenly spaced numbers over a specified interval  
`arr7 = np.linspace(start = 0, stop = 5, num = 10, endpoint = True)`# creates an array of 10 elements with evenly spaced numbers from 0 to 5 (including 5).  

---
**Array of Random Numbers**  
`np.random.rand(5)` # creates an array of 5 random numbers from 0 to 1  
`np.random.randn(5,5)` # creates a 5X5 matrix of random numbers from -1 to # 1  
`np.random.randint(1,100)` # returns a number between 1 and 100  
`np.random.randint(1,100,10)` # returns an array of 10 numbers between 1 and 100  
`arr = np.arange(25)` # returns an array of 25 elements from 0 to 25 (exclusive)  

--- 
**Indexing**  
`arr[8]` # returns element at 8th index  
`arr[1:5]` # returns elements of 1st to 5th (excluding) index  
`arr2d[0][0]` # returns element at 0th row and 0th column  
`arr2d[:2,1:]`  

---
**Operations**  
`arr-arr`  
`arr+5`  
`arr*arr`  
`1/arr` # ensure that none of the elements has value zero  
`np.sqrt(arr)`  
`np.exp(arr)`  
`np.sin(arr)`  
`np.log(arr)`  
  
---
**Other functions**  
`arr.max()` # returns maximum element of array  
`arr.min()` # returns minimum element of array  
`arr.argmax()` # returns index of maximum element  
`arr.argmin()` # returns index of minimum element  
`arr.shape()` # returns the shape of array  
`arr.dtype()` # returns the type of array  
`arr1 = arr.copy()` # initialises a copy of arr array to arr1    