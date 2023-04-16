# MATRICES & LIST COMPREHENSION

## MATRICES
A matrix is a way of representing numbers, symbols, or expressions in a 2-dimensional array. In python, we can create a matrix using a list within a list data structure. While there are external libraries that can help with creating matrices, we will use the built-in Python features. 

Matrices are important in math; particularly Calculus, Vectors, & Linear Algebra. 

![image](https://user-images.githubusercontent.com/128660559/232326879-a6d6d705-7884-4ca7-8219-27dca773828c.png)

```python

# Code Representation of Matrix A

matrix_A = [
    [1, 2, 3, 4],
    [5, 6, 7, 8]
]

print('Row 1: %s' % matrix_A[0])
print('Value at Row 2 Column 2: %s' % matrix_A[1][1])

```

Matrix A in Python is represented using a list within a list with two rows and four columns. Accessing specific rows or values in the matrix is done through indexing. Here are some important points to remember:
- Follow the rules of a regular matrix, including having the same number of values in each row and column
- Ensure that all items in the 2D list have the same data types
- Indexing starts at 0 in Python, meaning that the first row is actually located at matrix_A[0]


## LIST COMPREHENSION
List comprehension is a concise method for creating a list in Python. It's often used when creating a list that results from applying some operations to all items in a sequence. It is also useful whent he list is created from another iterable data or when the list is a member of another iterable data that meets a specific condition.

Here are 2 codes that aim to create a list which squares all the numbers from 0-9.
```python
# OLD METHOD

squares = []
for i in range(10):
    squares.append(i ** 2)
    
print('Our result: %s' % squares)
```
```python
# LIST COMPREHENSION

squares = [i**2 for i in range (10)]
print('Our result: %s' % squares)
```
This example demonstrates the use of list comprehension in Python to create a list that squares all the numbers from 0 to 9. The old method using a for loop to append the values to an empty is shown first. Below it, list comphrension consists of a square bracket containing an expression that describes the list, followed by one or more for clauses to explain its members, and optionally, zero or more clauses depending on the complexity of the list. 
