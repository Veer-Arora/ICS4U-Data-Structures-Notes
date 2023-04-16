# TUPLES

## WHAT ARE TUPLES?
Tuples are a data structure in Python that are immutable and allow for different data types as items. They are iterable and nestable, similar to a list within a list. Tuples are declared using parenthesis and can be empty for contain a single item with a comma. They can be sliced and indexed using square brackets.


Basic Tuples:

```python
tup = ('C', ' Java', 'Python')
empty_tup = ()
single_tup = ('Veer',)

print(tup)
print(empty_tup)
print(single_tup)

```

Tuple Operators 

```python
# Concatenation: Joining two tuples
a = (1,2,3)
b = (4,5,6)
concat_result = a + b
print('a+b:', concat_result)


# Repetition: Repeating a list multiple times
c = ('Hi!',)
repet_result = c * 3
print('c*3', repet_result)

# Membership: Check if a value exists in a tuple
d = a + b + c
print('d:', d)
print('\'Hi!\' in d:', 'Hi!' in d)
print('7 in d:', 7 in d)

```

Tupe & Python

```python

# PACKING & UNPACKING

var_1 = 2
var_2 = 3
var_3 = 5

prime = var_1, var_2, var_3

print('Packed prime values:', prime)

# Unpacking and Repacking
fib = (0, 1, 1, 2, 3, 5, 8)

fib_0, fib_1, fib_n = fib[0], fib[1], fib[2:]
print('fib_0:', fib_0)
print('fib_1:', fib_1)
print('fib_n:', fib_n)

```

This code demonstrates the concept of packign and unpacking in Python. Packing is the process of putting multiple values into a single variable, wheras unpacking is the opposite; extracting values from a single variable and assigning them to multiple varibales. The first part of the code packs three variables into a single typle called 'prime' and prints it. The second unpacks the first two values of the 'fib' tuple into seperate variables and the remaining values are packed into another tuple called 'fib_n'. The values of the unpacked variabled and 'fib_n' are then printed. 
