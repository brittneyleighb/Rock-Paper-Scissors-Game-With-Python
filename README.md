# Rock-Paper-Scissors-Game-With-Python

This is a simple tutorial I followed with Free Code Camp to practice some fundamentals of Python, 
such as variables, strings, defining and calling functions, etc.

Here are some of my notes:
### F-Strings

Creating a function: Can add data to the function.

def check_win(player, computer)

If statement - if statement is true, the following code with execute

A single equal sign is the assignment operator, == two means to equal like in an equation

== equals

!= does not equal

<= less than or equal to

>= greater than or equal to

concatenate simply means you can combine strings

*With programming there can be a lot of ways to do one thing* like spoken languages!

The f-string can make your code your condensed (look better) and use less code.

### Refactoring

The process of restructuring code while keeping the original functionality (to make it more simple/beautiful).

elif is short for else if

Structure for list is 

- if
- elif
- elif
- else

Once something is “returned” in code, the rest of code does not run (such as in else if statements).

### Calling the get_choices function/Accessing Dictionary Values

This is how we access a specific element in a dictionary.

choices = get_choices() This is a dictionary we are calling

choices = {"player": "rock", "computer": "paper"}  
p_choice = choices["player"] The brackets are to get the value of the player, “player” is the key (with the value of rock as defined in the brackets).

## Random Questions

### **What does “import random” mean in Python code?**

In Python, `import random` is a statement used to bring in the functionality of the `random` module into your code.

The `random` module provides various functions for generating random numbers, selecting random elements from sequences, and other randomization-related operations.

Once you import the `random` module using `import random`, you can use its functions in your code. For instance, you can generate random numbers, shuffle sequences, or select random elements from a list.

Here's an example demonstrating the use of the `random` module to generate a random number:

```python
import random

# Generate a random number between 1 and 10
random_number = random.randint(1, 10)
print(random_number)

```

In this case, `random.randint(1, 10)` generates a random integer between 1 and 10 (inclusive) and assigns it to the variable `random_number`. The `random` module's functionality becomes available after importing, allowing you to utilize its functions throughout your Python script.

### **What does it mean to “call a function” in Python?**

In Python, "calling a function" refers to executing or invoking a block of code that is encapsulated within a function. When you define a function, you're essentially creating a reusable block of code that can be executed multiple times by calling its name followed by parentheses "()". This triggers the execution of the code within the function's body.

For example, consider a simple function that adds two numbers:

```python
def add_numbers(a, b):
    return a + b

```

To call this `add_numbers` function and use it to add, let's say, 2 and 3:

```python
result = add_numbers(2, 3)
print(result)  # Output will be 5

```

Here, `add_numbers(2, 3)` is the function call. The values `2` and `3` are passed as arguments to the function, and the result of the addition is returned.

Functions in Python can accept arguments (inputs) and optionally return values (outputs). Calling a function is essentially instructing Python to execute the code defined within that function.

### **In my code the functions are defined as:**

def get_choices():
player_choice = input("Enter a choice (rock, paper, scissors: ")
options = ["rock", "paper", "scissors"]
computer_choice = random.choice(options)
choices = {"player": player_choice, "computer": computer_choice}

**With to “call the function” as:**

return choice

### What does it mean to “pass a value” from a dictionary key in Python code?

In Python, when we talk about passing in a value from a dictionary key, it generally means retrieving the value associated with a specific key within a dictionary and using that value in some way within your code.

A dictionary in Python is a collection of key-value pairs, where each key is unique and maps to a corresponding value. To access a value associated with a particular key in a dictionary, you simply reference the key within square brackets `[]`.

For example:

```python
my_dict = {'key1': 100, 'key2': 200, 'key3': 300}

# Accessing the value associated with 'key2'
value = my_dict['key2']
print(value)  # Output: 200

```

In the code above, `my_dict['key2']` retrieves the value `200` associated with the key `'key2'`.

Passing in a value from a dictionary key essentially means using the value associated with a specific key in subsequent operations or passing it as an argument to a function, depending on the context of your code.

For instance, you might use the value from a dictionary key as an input for a function:

```python
# Using the value associated with 'key3' in a calculation
result = my_dict['key3'] * 2
print(result)  # Output: 600

```

This code takes the value associated with `'key3'` (which is `300`) and multiplies it by `2`, storing the result in the `result` variable.

Passing in a value from a dictionary key involves accessing and utilizing the associated value for various operations or assignments within your Python code.

**In my code in Replit it is:**

choices = get_choices()
result = check_win(choices["player"], choices["computer"])
print(result)
