[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15372683&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a high-level programming language known for its simplicity and readability.Key features include: 
   1. Easy to learn.
   2. Supports multiple programming paradigms.
   3. Scalable.
   It is effective in various sectors such as :
   1. Web development
   2. Machine learning
   3. Automation and scripting

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

Windows:

Download the latest version of Python from the official website (https://www.python.org/downloads/) and run the installer.
During the installation process, make sure to check the box that says "Add Python to PATH" to allow Python to be accessible from the command line.
Once the installation is complete, open the Command Prompt and type 'python --version' to verify that Python is installed.
To set up a virtual environment, install the virtualenv package by running 'pip install virtualenv' in the Command Prompt.
Create a new virtual environment by navigating to your project directory and running 'virtualenv venv'.
Activate the virtual environment by running 'venv\Scripts\activate' in the Command Prompt.
macOS:

macOS typically comes with Python pre-installed. However, it's recommended to install the latest version using Homebrew or the official Python installer.
To install Python using Homebrew, run 'brew install python' in the Terminal.
Verify the installation by typing 'python3 --version' in the Terminal.
To set up a virtual environment, install the virtualenv package by running 'pip install virtualenv'.
Create a new virtual environment by running 'virtualenv venv' in the Terminal.
Activate the virtual environment by running 'source venv/bin/activate' in the Terminal.
Linux:

Most Linux distributions come with Python pre-installed. To install the latest version, use the package manager specific to your distribution (e.g., apt for Debian-based systems).
Install Python by running 'sudo apt install python3' in the terminal.
Verify the installation by typing 'python3 --version' in the terminal.
To set up a virtual environment, install the virtualenv package by running 'pip install virtualenv'.
Create a new virtual environment by running 'virtualenv venv' in the terminal.
Activate the virtual environment by running 'source venv/bin/activate' in the terminal.


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, world!")

print(): A built-in function used to output text to the console.
"Hello, world!": A string literal enclosed in double quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

Basic Data Types in Python:

Integer (int): Represents whole numbers without any decimal point.
Floating-point (float): Represents numbers with a decimal point.
String (str): Represents text data enclosed in single (' ') or double (" ") quotes.
Boolean (bool): Represents True or False values.
List: Represents an ordered collection of items that can be of different data types.
Tuple: Represents an ordered, immutable collection of items.
Dictionary: Represents a collection of key-value pairs.
Set: Represents an unordered collection of unique elements.

# Integer
x = 10

# Floating-point
y = 5.5

# String
name = "Alice"

# Boolean
is_student = True

# List
numbers = [1, 2, 3, 4, 5]

# Tuple
coordinates = (10, 20)

# Dictionary
person = {'name': 'Bob', 'age': 30}

# Set
unique_numbers = {1, 2, 3, 4, 5}

# Printing variables
print(x)  # Output: 10
print(y)  # Output: 5.5
print(name)  # Output: Alice
print(is_student)  # Output: True
print(numbers)  # Output: [1, 2, 3, 4, 5]
print(coordinates)  # Output: (10, 20)
print(person)  # Output: {'name': 'Bob', 'age': 30}
print(unique_numbers)  # Output: {1, 2, 3, 4, 5}

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

1. Conditional Statements: Allow you to execute different blocks of code based on certain conditions
The if statement is used to check a condition and execute a block of code if the condition is true. Optionally, you can use else and elif statements for additional conditions.
Example:
       # If-Else statement
score = 85

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("Fail")

2. Loops: Are used to execute block of code repeatedly. The for loop is used to iterate over a sequence or an iterable object.
Example:
        # For loop
fruits = ["apple", "banana", "orange"]

for fruit in fruits:
    print(fruit)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions in Python are reusable blocks of code that perform a specific task. They allow you to organize your code into logical units, making it easier to read debug and maintain.

def calculate_sum(a, b):
    """
    Function to calculate the sum of two numbers.
    
    Args:
        a (int): First number
        b (int): Second number
        
    Returns:
        int: Sum of a and b
    """
    return a + b


    # Calling the calculate_sum function
result = calculate_sum(5, 3)
print("The sum is:", result)  # Output: The sum is: 8

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Lists: Are ordered collections of items that contain elements of any data type.
       Elements in a list are indexed starting from 0.
       Lists are created using square brackets [].

Dictionaries: Are unordered collections of key-value pairs.
             Each element is stored as a key-value pairs.
             Are created using curly braces {}.


   # Creating a list of numbers
numbers_list = [1, 2, 3, 4, 5]

# Creating a dictionary with key-value pairs
person_info = {
    'name': 'Alice',
    'age': 30,
    'is_student': True,
    'hobbies': ['reading', 'coding']
}

# Accessing elements in the list
print(numbers_list[2])  # Output: 3

# Accessing values in the dictionary
print(person_info['name'])  # Output: Alice

# Modifying an element in the list
numbers_list[3] = 10

# Modifying a value in the dictionary
person_info['age'] = 35

# Adding elements to the list
numbers_list.append(6)

# Adding a new key-value pair to the dictionary
person_info['city'] = 'New York'

# Removing an element from the list
numbers_list.remove(2)

# Removing a key-value pair from the dictionary
del person_info['is_student']

# Printing the modified list and dictionary
print(numbers_list)  # Output: [1, 3, 10, 5, 6]
print(person_info)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling is a way to deal with errors that occur during the execution of a program.

# Example of handling division by zero error
try:
    num1 = 10
    num2 = 0
    result = num1 / num2
    print("Result:", result)
except ZeroDivisionError:
    print("Error: Cannot divide by zero")
finally:
    print("End of the program")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

A module is a file containing python code, typically functions, classes and variables that can be imported and used in other python scripts.
A package is a collection of modules that are organized in a directory structure and can be imported as a whole.
To import a module in python, you use the import keyword followed by the module name. Once imported, you can access the function, classes and variables defined in the module by using the dot notation 
(module_name.element_name).   

     
import math

# Using functions from the math module
print(math.sqrt(16))  # Output: 4.0 (square root of 16)
print(math.pi)        # Output: 3.141592653589793 (value of pi)
print(math.factorial(5))  # Output: 120 (factorial of 5)

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

To read from a file, you can use functions like open() to open the file, read() to read its content and close() to close the file.
To write to a file, you can use the functions like open() to open file in write mode, write() to write content to the file and close() to close the file.

# Reading from a file and printing its content
with open('sample.txt', 'r') as file:
    content = file.read()
    print(content)


data = ['Hello', 'Python', 'World']

with open('output.txt', 'w') as file:
    for item in data:
        file.write(item + '\n')

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].



