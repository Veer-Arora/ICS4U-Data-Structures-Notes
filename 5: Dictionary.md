# DICTIONARY

## WHAT IS DICTIONARY?
Dictionary is a date type that stores a collection of (key,value) pairs, where each possible key appears at most once. Common operations with dictionaries include adding a pair, removing a pair, modifying an existing pair, and looking up a vlaue associated with a particular key. Dictionaries are similar to hash tables and search trees. 

Example 1:

```python
# Dictionary Example

sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

print('Sammy dict:', sammy)
print('Username:', sammy['username'])
print('Online Status:', sammy['online'])
print('Follower Count:', sammy['followers'])

```
A dictionary in Python stores key-value pairs where keys must be unique, immutable and newest created item with a duplicate key supersedes the previous declaration. Values of a dictionary can be of any data type. 

- Dictionaries can be updated by modifying existing values by referencing the key
- Newkey-value pairs can be added to a dictionary by creating a new key and assigning a value to it
- Values for an existing key can be overwritten by referencing the key and recreating the value for it

Here an example of Updating:

```python

sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

sammy['followers'] += 10 
sammy['verified'] = True 
sammy['username'] = 'SammySammy'

print('Sammy Dict:', sammy)

```

Here's an example of Deleting: 

```python
sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

del sammy['followers'] 
print('followers key deleted:', sammy)

sammy.clear() # {} is considered an empty dict
print('emptying out a dictionary', sammy)
print('--\n\n')

del sammy
print('Deleting sammy, should create an error when referenced again', sammy)

```

Deletion with Dictionary can be done by deleting a key, which will also delete the associated value. The entire dictionary can also be emptied out or deleted entirely. 

Here's an example of some Dictionary Methods:

```python
# Dictionary Method Examples

sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

sammy_hidden = {
    'pwd' : 'qwerty',
    'location' : 'Toronto, Ontario'
}

# printing all the keys of a dict
print('Sammy Dict Keys:', sammy.keys()) # notice how it prints

sammy_keys = list(sammy.keys()) # we can listify the .keys() returned
print('List of sammy_keys', sammy_keys)
print('--')

# printing all the values of a dict
print('Sammy Dict Values:', sammy.values())
print('Sammy Dict Values as a list:', list(sammy.values()))
print('--')

# printing key, value pair of a dict
print('Sammy Dict key, value pairs:', sammy.items())
print('Sammy Dict key, value pairs as a list:', list(sammy.items()))
print('--')

# getting a value from a dict
print('Sammy followers value:', sammy.get('followers'))
print('Same as:', sammy['followers'])
print('--')

# updating / extending a dictionary
sammy.update(sammy_hidden)

print('Sammy extended with its hidden values:', sammy)

```

In summary, dictionaries are a powerful and verstalie data strcuture in Python that allow us to store and manipulate the data using key-value pairs. They have several useful properties such as uniqueness of keys and the ability to store any data type as values. We can add, modify, and delete items in a dictionary, making it a flexible tool for data management. Understanding dictionaries is an essential part of Python programming and can be used in a wide range of applications
