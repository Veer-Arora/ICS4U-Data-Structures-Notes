# MAP & FILTER

## MAP FUNCTION
The map function applies a function to iterable data, using the format map(function_name, sequence), where the function can be any built-in or self-made function that returns a desired value, and the sequence can be any iterable data type. 

Here's an example:

```python

def square(num):
    return num ** 2

array = list(range(1,11))
square_array = list(map(square, array))

print('Original Array:', array)
print('Array Squared:', square_array)

```

This code defines a function called square that takes a number as input and returns its square. It then creates an array of numbers from 1 to 10 using the range funtion. The mpa function is then used to apply the 'square' function to eahc element of the array, creating a new list of the squarred values. Finally, the original array and the squarred array are printed. The map function is used to apply a function to each element in a sequence and return a new sequence with the results. 


## FILTER FUNCTION
The filter function allows us to filter out items from a data set that satisfy a specific condition. We pass a boolean-returning function and a sequence to the filter() function. The function provided should be able to handle the items inside the sequence as its arguments. 

Here's an example:

```python

# Palindromic Numbers from 1 to 10000

def isPalindrome(x):
    return x == x[::-1]

array = list(range(1,10000))

palindromic_numbers = list(map(int, filter(isPalindrome, map(str, array))))
print('Palindromic Numbers from 1 to 10,000', palindromicNumbers)

```
The code creates a list of palindromix numbers from 1 ot 10,000 using the filter and map functions. The function 'isPalindrome' checks if a numbers is a palinrome by comparing it to its reverse. The map function is used to convert the integer array into a string array. Then, the filter function is used to filter out only the palindromic numbers from the string array. Finally, the filtered strig array is mapped back to integers and converted into a list of palindromic numbers. The result is printed as "Palindromic Numbers from 1 to 10,000" along with the list of palindromic numbers. 


