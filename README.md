# Python.

## Installation
1. **Install Anaconda**: [Anaconda Installation Guide](https://docs.anaconda.com/anaconda/install/windows/). After installation,
   -> Verify it by typing `python` and then `exit()` in the command prompt.
2. **Activate Base Environment**: Use the command `activate base` to activate the default virtual environment.
3. **Jupyter Notebook**: Run `jupyter notebook` to launch the web-based IDE in your local environment.
4. **Check Python Version**: Inside Jupyter notebook, use `!python --version` to check the Python version.

### Other Useful Commands
- Locate Python: `whereis python`  
- Find active Python: `which python`

## Calculations / Built-in Functions

1. **Print Statement**:  
   `print("Hello world!")`  
   **Explanation**: Prints the content inside the quotes.  
   **Output**: `Hello world!`

2. **Length of String**:  
   `len("Hello world!")`  
   **Explanation**: Returns the length of the string, including spaces.  
   **Output**: `12`

3. **Mathematical Calculation (BODMAS)**:  
   `print(4.5 - 2 * (4 / 7))`  
   **Explanation**: Follows the BODMAS rule for calculations. First, division happens (`4/7`), then multiplication by 2, and finally subtraction from 4.5.  
   **Output**: `2.857142857142857`

4. **Absolute Value**:  
   `abs(-17)`  
   **Explanation**: Returns the absolute (positive) value of a number.  
   **Output**: `17`

5. **Type Check**:  
   `type(17.5)`  
   **Explanation**: Returns the data type of the given value. In this case, it’s a float (decimal number).  
   **Output**: `<class 'float'>`

6. **Rounding**:  
   `round(17.4)`  
   **Explanation**: Rounds the given number to the nearest integer. Since 17.4 is closer to 17 than 18, it rounds down.  
   **Output**: `17`

7. **Maximum Value**:  
   `max(9, 5, 6, 12, 23)`  
   **Explanation**: Returns the maximum value from the given list of numbers.  
   **Output**: `23`

8. **Minimum Value**:  
   `min(9, 5, 6, 12, 23)`  
   **Explanation**: Returns the minimum value from the given list of numbers.  
   **Output**: `5`

## Variables

Variables are containers that hold values. You can use characters `a-z`, `A-Z`, numbers `0-9`, and the underscore `_` to name them.

```python
salary = 28000                     # Salary assigned to the variable
house_rent = 10000                 # House rent assigned to the variable
food_exp = 5000                    # Food expenses assigned to the variable
total_expense = house_rent + food_exp  # Total expenses calculated
print(total_expense)               # Output: 15000

saving = salary - total_expense     # Savings calculated
print("My total saving of this month is", saving)  # Output: My total saving of this month is 13000
```

## Data Types

Python supports various data types:

```python
# Int: Stores integer values (whole numbers).
age = 25
print(type(age))  # Output: <class 'int'>

# Float: Stores floating-point numbers (numbers with decimals).
height = 5.9
print(type(height))  # Output: <class 'float'>

# Complex: Stores complex numbers (real and imaginary parts).
complex_num = 3 + 5j
print(type(complex_num))  # Output: <class 'complex'>

# Bool: Stores Boolean values: True or False.
is_active = True
print(type(is_active))  # Output: <class 'bool'>

# Str: Stores string values (sequences of characters).
name = "John"
print(type(name))  # Output: <class 'str'>
```

## Strings

Strings in Python are used to store text, and various operations can be performed on them.

```python
# Concatenation of strings using different quotes
print('python ' + "is" + """awesome""")  # Output: python is awesome

# String repetition
print('python' * 3)  # Output: pythonpythonpython

# Example with user input
Q = "What did you have for lunch?"
A = input(Q)  # Takes user input
print("You had " + A + "! That sounds delicious")

# Escape characters using backslash (\)
print("I\'m learning Python")  # Output: I'm learning Python

# Special characters
print("Hello\tWorld")  # Output: Hello    World (tab space)
print("Hello\nWorld")  # Output: Hello (new line) 
                       #          World

# Triple quotes for multi-line strings
print("""This is a 
multi-line string""")  # Output:
# This is a
# multi-line string

# String formatting
my_var = 'blue'
print("The sky is " + my_var)  # Output: The sky is blue
print(f"The sky is {my_var}")  # Output: The sky is blue (f-string formatting)
print("The sky is {}".format(my_var))  # Output: The sky is blue (format method)
```

## Lists

Lists in Python are used to store multiple items in a single variable. They are ordered, changeable, and allow duplicate values.

```python
# Creating a list
fruits = ["apple", "banana", "cherry"]
print(fruits)  # Output: ['apple', 'banana', 'cherry']

# Accessing list items
print(fruits[0])  # Output: apple (access first element)
print(fruits[-1])  # Output: cherry (access last element)

# Changing list items
fruits[1] = "blueberry"
print(fruits)  # Output: ['apple', 'blueberry', 'cherry']

# List length
print(len(fruits))  # Output: 3 (number of items in the list)

# Adding items to the list
fruits.append("orange")
print(fruits)  # Output: ['apple', 'blueberry', 'cherry', 'orange']

# Inserting items into the list
fruits.insert(1, "mango")
print(fruits)  # Output: ['apple', 'mango', 'blueberry', 'cherry', 'orange']

# Removing items from the list
fruits.remove("cherry")
print(fruits)  # Output: ['apple', 'mango', 'blueberry', 'orange']

# Popping the last item
fruits.pop()
print(fruits)  # Output: ['apple', 'mango', 'blueberry']

# Sorting the list
fruits.sort()
print(fruits)  # Output: ['apple', 'blueberry', 'mango']

# Reversing the list
fruits.reverse()
print(fruits)  # Output: ['mango', 'blueberry', 'apple']
```

## Tuples

Tuples in Python are similar to lists but are immutable (i.e., they cannot be changed after their creation). They are defined using parentheses `()` instead of square brackets `[]`.

```python
# Creating a tuple
fruits = ("apple", "banana", "cherry")
print(fruits)  # Output: ('apple', 'banana', 'cherry')

# Accessing tuple items
print(fruits[0])  # Output: apple
print(fruits[-1])  # Output: cherry

# Tuples are immutable (you cannot change items)
# fruits[1] = "blueberry"  # This will raise a TypeError

# Tuple length
print(len(fruits))  # Output: 3

# Unpacking tuples
fruit1, fruit2, fruit3 = fruits
print(fruit1)  # Output: apple
print(fruit2)  # Output: banana
print(fruit3)  # Output: cherry

# Tuples with one item (comma needed)
single_item_tuple = ("apple",)
print(type(single_item_tuple))  # Output: <class 'tuple'>

# Tuple methods (limited compared to lists)
print(fruits.count("apple"))  # Output: 1 (counts occurrences)
print(fruits.index("banana"))  # Output: 1 (returns the index of an item)
```

## Sets

Sets in Python are unordered collections of unique items. They are defined using curly braces `{}`.

```python
# Creating a set
fruits = {"apple", "banana", "cherry"}
print(fruits)  # Output: {'banana', 'apple', 'cherry'}

# Sets do not allow duplicates
fruits = {"apple", "banana", "cherry", "apple"}
print(fruits)  # Output: {'banana', 'apple', 'cherry'} (duplicate 'apple' is removed)

# Checking if an item is in a set
print("apple" in fruits)  # Output: True

# Adding an item to a set
fruits.add("orange")
print(fruits)  # Output: {'banana', 'apple', 'cherry', 'orange'}

# Adding multiple items to a set
fruits.update(["mango", "grapes"])
print(fruits)  # Output: {'banana', 'apple', 'cherry', 'orange', 'mango', 'grapes'}

# Removing an item from a set
fruits.remove("banana")
print(fruits)  # Output: {'apple', 'cherry', 'orange', 'mango', 'grapes'}

# Sets are unordered and do not support indexing
# print(fruits[0])  # This will raise a TypeError

# Set operations (union, intersection, difference)
set1 = {"apple", "banana", "cherry"}
set2 = {"google", "microsoft", "apple"}

# Union of sets
print(set1 | set2)  # Output: {'apple', 'banana', 'cherry', 'google', 'microsoft'}

# Intersection of sets
print(set1 & set2)  # Output: {'apple'}

# Difference of sets
print(set1 - set2)  # Output: {'banana', 'cherry'}
```

## Dictionaries

Dictionaries in Python are collections of key-value pairs. Each key is unique, and the values can be accessed via their corresponding keys. They are defined using curly braces `{}` with key-value pairs separated by a colon `:`.
