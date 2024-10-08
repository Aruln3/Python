# Python

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
print("My total saving of this month", saving)  # Output: My total saving of this month 13000

