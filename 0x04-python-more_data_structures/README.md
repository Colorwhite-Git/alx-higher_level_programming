#Python Data Structures

Python programming is awesome for several reasons. It's known for its simplicity and readability, making it easier for beginners to learn and for experienced developers to write clean and maintainable code. Its extensive libraries and frameworks cover a wide range of applications from web development and data analysis to artificial intelligence and scientific computing. Python's versatility, ease of use, and strong community support contribute to its popularity and effectiveness in various fields.

Sets in Python are unordered collections of unique elements. They are defined using curly braces {} and can contain various immutable data types like integers, strings, tuples, etc. Sets do not allow duplicate elements, and they are mutable, meaning you can modify them after creation. Here's an example:



my_set = {1, 2, 3, 4, 5}
Common methods of sets include:

add: Adds an element to the set.
remove: Removes a specified element from the set.
discard: Removes a specified element from the set if it is present.
pop: Removes and returns an arbitrary element from the set.
union: Returns a new set containing elements from both sets without duplicates.
intersection: Returns a new set containing common elements from two sets.
Sets are useful when you need to perform mathematical operations like finding unique elements, intersections, or unions efficiently.

Use sets when you need uniqueness or when you need to perform set operations like intersection, union, or difference efficiently. Lists, on the other hand, are ordered collections that allow duplicates and are more suitable for scenarios where the order of elements matters or duplicates are needed.

To iterate over a set, you can use a loop, such as a for loop:



my_set = {1, 2, 3, 4, 5}
for element in my_set:
    print(element)
Dictionaries in Python are collections of key-value pairs. They are defined using curly braces {} and consist of keys and their associated values. Keys must be unique and immutable (strings, numbers, tuples), while values can be of any data type. Dictionaries are unordered, meaning they don’t retain the order of elements.



my_dict = {'name': 'Alice', 'age': 30, 'city': 'New York'}
Dictionaries are great for storing and accessing data using descriptive keys rather than indices, especially when you have pairs of related information.

Use dictionaries when you need to associate unique keys with values or when you want to store data as key-value pairs. Lists or sets are used for collections without key-value associations.

A key in a dictionary is a unique identifier used to access its associated value. Each key in a dictionary must be unique.

To iterate over a dictionary, you can use a for loop:



my_dict = {'name': 'Alice', 'age': 30, 'city': 'New York'}
for key, value in my_dict.items():
    print(key, value)
A lambda function in Python is an anonymous (unnamed) function defined using the lambda keyword. It is a way to create small, one-line functions without using the def keyword. Lambda functions can take any number of arguments but can only have one expression.



addition = lambda x, y: x + y
print(addition(2, 3))  # Output: 5
The map, reduce, and filter functions are higher-order functions commonly used with lambda functions:

map: Applies a function to each item in an iterable.
reduce: Performs a computation on a list and returns the result.
filter: Filters elements from an iterable based on a function's condition.
For example:


numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, numbers))  # squares each number in the list
total = reduce(lambda x, y: x + y, numbers)  # adds all numbers in the list
evens = list(filter(lambda x: x % 2 == 0, numbers))  # filters out odd numbers
