## Python Fundamentals
Python is a high-level, interpreted programming language that was created by Guido van Rossum and first released in 1991. Its design philosophy emphasizes code readability and simplicity, making it an excellent choice for both beginners and experienced developers. Over the years, Python has undergone significant development and improvement, with major releases adding new features and optimizations. The language’s versatility and ease of use have made it popular in various domains, including web development, data science, artificial intelligence, scientific computing, automation, and more. Python’s extensive standard library and active community contribute to its widespread adoption, making it one of the most popular programming languages in the world today.

## Printing text
```{python}
print("Hello, World!")
```
## Printing multiple values
```{python}
x = 5
y = 10
print("The value of x is:", x, "and the value of y is:", y)
```

## Assigning values to variables
```{python}
a = 10
b = 20.5
name = "Alice"
```
## Printing the values
```{python}
print("Values Stored in the Variables:")
print(a)
print(b)
print(name)
```
## Taking input from the user
```{python}
name = input("Enter usr name: ")

 Python Programming Style
 Indentation
 if a > b:
    print("a is greater than b")
else:
    print("b is greater than or equal to a")                         
print("Hello, " + name + "!")
```
## Taking numerical input
```{python}
age = int(input("Enter usr age: "))
print("us are", age, "years old.")
```
## Program to calculate the sum of two numbers
```{python}
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
# Calculate sum
sum = num1 + num2
# Display the result
print("The sum of", num1, "and", num2, "is", sum)
student_name = "John"
total_score = 95
```
## Creating strings with different types of quotes
```{python}
single_quoted = 'Hello, World!'
double_quoted = "Hello, World!"
multiline_string = """This is a
multiline string"""
# Accessing the first item
first_fruit = fruits[0]  # Output: "apple"
# Accessing the last item
last_fruit = fruits[-1]  # Output: "cherry"
```
## Using list methods
```{python}
numbers = [5, 2, 9, 1]

numbers.append(4)     # numbers is now [5, 2, 9, 1, 4]
numbers.sort()        # numbers is now [1, 2, 4, 5, 9]
numbers.reverse()     # numbers is now [9, 5, 4, 2, 1]
first_number = numbers.pop(0)  # first_number is 9, numbers is now [5, 4, 2, 1]

# Using tuple methods
numbers = (1, 2, 3, 1, 2, 1)

# Counting occurrences of an item
count_1 = numbers.count(1)  # Result: 3

# Finding the index of an item
index_2 = numbers.index(2)  # Result: 1
# Using dictionary methods
keys = student.keys()        # Result: dict_keys(['name', 'age', 'graduation_year'])
values = student.values()    # Result: dict_values(['Alice', 22, 2024])
items = student.items()      # Result: dict_items([('name', 'Alice'), ('age', 22), ('graduation_year', 2024)])
name = student.get("name")  # Result: "Alice"
age = student.pop("age")    # Result: 22
# Checking membership
has_apple = "apple" in fruits  # Output: True

# Since frozenset is immutable, us cannot use add() or remove() methods
# Using frozen set methods
set1 = frozenset([1, 2, 3])
set2 = frozenset([3, 4, 5])

# Getting the difference
difference = set1.difference(set2)  # Result: frozenset({1, 2})

# Getting the intersection
intersection = set1.intersection(set2)  # Result: frozenset({3})

# Getting the union
union = set1.union(set2)  # Result: frozenset({1, 2, 3, 4, 5})

# Getting the symmetric difference
symmetric_difference = set1.symmetric_difference(set2)  # Result: frozenset({1, 2, 4, 5})
```

## Control Structures in Python
Control structures in Python allow us to control the flow of execution in our programs. They help manage decision-making, looping, and the execution of code blocks based on certain conditions. Python provides several key control structures: if statements, for loops, while loops, and control flow statements like break, continue, and pass.

## Conditional Statements
Conditional statements are used to execute code based on certain conditions. The primary conditional statement in Python is the if statement, which can be combined with elif and else to handle multiple conditions.

#### syntax
```{python}
if condition:
    # Code block to execute if condition is True
elif another_condition:
    # Code block to execute if another_condition is True
else:
    # Code block to execute if none of the above conditions are True
```
```{python}
 age = 20

if age < 18:
    print("us are a minor.")
elif age < 65:
    print("us are an adult.")
else:
    print("us are a senior citizen.")
```
## Looping Statements
Looping statements are used to repeat a block of code multiple times. Python supports for loops and while loops.

## For loop

The for loop iterates over a sequence (like a list, tuple, or string) and executes a block of code for each item in the sequence.
```{python}
for item in sequence:
    # Code block to execute for each item
```

```{python}
# Iterating over a list
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

```{python}
# Counting from 0 to 4
count = 0
while count < 5:
    print(count)
    count += 1

# Output: 0 1 3 4
```
## Control flow statements
  Control flow statements alter the flow of execution within loops and conditionals.

  ## Break Statement 
  The break statement exits the current loop, regardless of the loop’s condition.

```{python}
for i in range(10):
    if i == 5:
        break
    print(i)
# Output: 0 1 2 3 4
```
## Continue Statement 
The continue statement skips the rest of the code inside the current loop iteration and proceeds to the next iteration.

```{python}
    for i in range(5):
    if i == 2:
        continue
    print(i)
# Output: 0 1 3 4

```

## Pass Statement
The pass statement is a placeholder that does nothing and is used when a statement is syntactically required but no action is needed.
```{python}
for i in range(5):
    if i == 3:
        pass  # Placeholder for future code
    else:
        print(i)
# Output: 0 1 2 4
```
 ## Functions in Python Programming
Functions are a fundamental concept in Python programming that enable code reuse, modularity, and organization. They allow us to encapsulate a block of code that performs a specific task, which can be executed whenever needed. Functions are essential for writing clean, maintainable, and scalable code, making them a cornerstone of effective programming practices.

#### What is a Function?
A function is a named block of code designed to perform a specific task. Functions can take inputs, called parameters or arguments, and can return outputs, which are the results of the computation or task performed by the function. By defining functions, us can write code once and reuse it multiple times, which enhances both efficiency and readability.

#### Defining a Functio 
In Python, functions are defined using the def keyword, followed by the function name, parentheses containing any parameters, and a colon. The function body, which contains the code to be executed, is indented below the function definition.

```{python}
def function_name(parameters):
    # Code block
    return result
```
##### Example
```{python}
 def greet(name):
    """
    Returns a greeting message for the given name.
    """
    return f"Hello, {name}!"
```

## Relevance of functions in Programming
1. Code Reusability : Functions allow us to define a piece of code once and reuse it in multiple places. This reduces redundancy and helps maintain consistency across our codebase.

2. Modularity : Functions break down complex problems into smaller, manageable pieces. Each function can be focused on a specific task, making it easier to understand and maintain the code.

3. Abstraction : Functions enable us to abstract away the implementation details. We can use a function without needing to know its internal workings, which simplifies the code we write and enhances readability.

4. Testing and Debugging : Functions allow us to test individual components of our code separately. This isolation helps in identifying and fixing bugs more efficiently.

5. Library Creation : Functions are the building blocks of libraries and modules. By organizing related functions into libraries, we can create reusable components that can be shared and utilized across different projects.

#### Stage 1: Define Functions in a Module
```{python}

# my_library.py

def add(a, b):
    """
    Returns the sum of two numbers.
    """
    return a + b

def multiply(a, b):
    """
    Returns the product of two numbers.
    """
    return a * b
```
#### Stage 2: Use the Library in Another Program
```{python}
# main.py

import my_library

result_sum = my_library.add(5, 3)
result_product = my_library.multiply(5, 3)

print(f"Sum: {result_sum}")
print(f"Product: {result_product}")
```
