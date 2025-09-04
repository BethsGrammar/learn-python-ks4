# Lesson 1: Introduction to Python
### Practice Exercises
Follow the instructions in each cell to test your understanding of today's lesson.
**Remember:** To run a cell in a real Jupyter Notebook, click on the cell and press `Shift + Enter`.
---
### A Note on `assert`
After you complete each exercise, you'll see a code block with an `assert` command. This command is a simple test that checks if a condition is `True`.
* If the condition is `True`, nothing happens and the test passes.
* If the condition is `False`, the program stops and shows an `AssertionError`.
Your goal is to write code that makes all the `assert` tests pass!


### Exercise 1: Basic Printing and Variables
1.  Create a variable called `favourite_colour` and set its value to a string of your favourite colour.
2.  Create a variable called `lucky_number` and set its value to a number between 1 and 100.
3.  On a new line, print the value of `favourite_colour`.
4.  On another new line, print the value of `lucky_number`.

```python
# Your code goes here:
favourite_colour = "Blue"
lucky_number = 42
print(favourite_colour)
print(lucky_number)

# --- Test ---
assert isinstance(favourite_colour, str), "Error: favourite_colour should be a string."
assert isinstance(lucky_number, int) or isinstance(lucky_number, float), "Error: lucky_number should be a number."
print("Exercise 1 Test Passed!")
```

### Exercise 2: Multiple Lines with `\n`
In the cell below, create a **single variable** called `rhyme_lines` that contains the following three lines as a single string, using the `\n` escape code:
"I am learning Python."
"It is fun and interesting."
"I can't wait to build a program!"
Then, print the `rhyme_lines` variable.

```python
# Your code goes here:
rhyme_lines = "I am learning Python.\nIt is fun and interesting.\nI can't wait to build a program!"
print(rhyme_lines)

# --- Test ---
expected_output = "I am learning Python.\nIt is fun and interesting.\nI can't wait to build a program!"
assert rhyme_lines == expected_output, "Error: The string does not match the expected format."
print("Exercise 2 Test Passed!")
```

### Exercise 3: Using Triple Quotes
In the cell below, create a **single variable** called `poem` and set its value to a multi-line string using triple quotes. The poem should be at least 3 lines long.

Then, print the `poem` variable.

```python
# Your code goes here:
poem = """
Twinkle, twinkle, little star,
How I wonder what you are.
Up above the world so high,
Like a diamond in the sky.
"""
print(poem)

# --- Test ---
assert isinstance(poem, str), "Error: The poem variable should be a string."
assert len(poem.strip().splitlines()) >= 3, "Error: The poem should have at least 3 lines."
print("Exercise 3 Test Passed!")
```

### Exercise 4: Variables and Constants
1.  Create a variable called `my_age` and set its value to your current age.
2.  Create a constant called `DAYS_IN_WEEK` and set its value to `7`.
3.  On a new line, print the value of `my_age`.
4.  On another new line, print the value of `DAYS_IN_WEEK`.

```python
# Your code goes here:
my_age = 15
DAYS_IN_WEEK = 7
print(my_age)
print(DAYS_IN_WEEK)

# --- Test ---
assert my_age > 0, "Error: Your age must be a positive number."
assert DAYS_IN_WEEK == 7, "Error: The value of DAYS_IN_WEEK is incorrect."
assert DAYS_IN_WEEK == 7, "Error: The value of DAYS_IN_WEEK is incorrect."
print("Exercise 4 Test Passed!")
```

### Exercise 5: Basic Math
1.  Create a variable called `apples` and set its value to `10`.
2.  Create a variable called `oranges` and set its value to `5`.
3.  Create a new variable called `total_fruit` that is the sum of `apples` and `oranges`.
4.  Print the value of `total_fruit`.
5.  Create a new variable called `product` that is the result of multiplying `25` by `3`.
6.  Print the value of `product`.

```python
# Your code goes here:
apples = 10
oranges = 5
total_fruit = apples + oranges
print(total_fruit)
product = 25 * 3
print(product)

# --- Test ---
assert total_fruit == 15, "Error: total_fruit should be 15."
assert product == 75, "Error: product should be 75."
print("Exercise 5 Test Passed!")
```