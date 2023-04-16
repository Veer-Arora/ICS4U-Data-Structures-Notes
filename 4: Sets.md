# SETS

## WHAT IS A SET?
A set data structure in Python is an unordered collected that contains unique elemtns only, making it a useful mathematical tool for handling collections of distinct objects. By following the operations and characteristics of mathematical sets, we can apply such structures in Python code. 


Example 1: How to Define a Set

```python
example_set1 = {1, 2, 3}
example_set2 = {'h','e','l','l','o'}

print('example_set1:', example_set1)
print('example_set2:', example_set2) 
print('--')

singleton_set = {7}
empty_set = set() 

print('Singleton:', singleton_set)
print('Empty Set:', empty_set)

```
The code intializes two sets, `example_set1` and `example_set2`, which contain unique elements. It then creates a `singleton_set` with a single element, and an empty set uisng the `set()` function.


Example 2: Disjoint

```python
# Disjoint Example
# .isdisjoint() is a set method to check for such property between two sets.

set1 = {1,2,3,4}
set2 = {5,6,7}
set3 = {1,2,3,4,5}

print('set1 intersect set2:', set1 & set2) 
print('set1 intersect set3:', set1 & set3)
print('--')
print('set 1 disjoint set 2 check:', set1.isdisjoint(set2)) 
print('set 1 disjoint set 3 check:', set2.isdisjoint(set3))

```
This code defines three sets: `set1`, `set2`, and `set3`, and check sif they are disjoint using the isdisjoint() set method. It also demonstrates the intersection of two sets using the ampersand symbol "&".


Example 3: Assignment Operation & Updating Methods

```python
# Union and Update
a = set('abracadabra')
b = set('alacazam')

a |= b # same as: a.update(b)
print('Union Update:', a)

# Intersection and Update
a = set('abracadabra')
b = set('alacazam')

a &= b # same as: a.intersection_update(b)
print('Intersection Update:', a)

# Difference and Update
a = set('abracadabra')
b = set('alacazam')

a -= b # same as: a.difference_update(b)
print('Difference Update:', a)

# Symmetric Difference and Update
a = set('abracadabra')
b = set('alacazam')

a ^= b # same as: a.symmetric_difference_update(b)
print('Symmeteric Difference Update:', a)

```
This is a way to affect an original set with another and assign the result back to the original set. The code demonstrates the use of set methods for set union, intersection, difference, and symmetric difference with their corresponding update methods. Each operation can be performed with either the '|' or '&' or '-' or '^' operator, respectively. The update methods modify the set in place, wheras the operators return a new set. 


Example 4: Set Comprehension

```python
def isPalindrome(x):
    return x == x[::-1]

nums = list(range(1,10000))
palindromic_set = {num for num in nums if isPalindrome(str(num))}

print('Palindromic Numbers Set from 1 to 10000:')
print(palindromic_set)

```

Overall:
- Sets aren't sliceable nor indexable
- Sets cannot have sets inside them
- Sets do not have order; nor order of insertion
- Sets cannot guarantee that their values will be in order
- Sets do not record a values position
