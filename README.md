[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15316809&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is an interpreted, object-oriented, high-level programming language with dynamic semantics.
Key features that make it popular among developers include its extensive standard library, dynamic typing, and support for multiple programming paradigms. 
Python is usually effective in web development like Django, data analysis and visualisation like Pandas, as well as machine learning like Tensorflow.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   To install Python for Windows:
      Go to the official Python website: python.org.
      Navigate to the Downloads section and choose the latest stable version for Windows.
      Click the download link to get the Python installer.
   To Run the Installer:
      Open the downloaded Python installer file.
      Ensure you check the box that says "Add Python to PATH". This will make it easier to run Python from the command line.
      Click "Install Now" to begin the installation process.
   To verify installation of Python:
      Open git bash and in it type the command:
         python --version
      When you press enter it will give you the version of python which you have installed, which indicates that you have successfully installed it.
   To set up an virtual environment:
      In git bash navigate to your project directory using the cd command.
      Create a virtual environment by typing this command:
         python -m virtualenv yourvenv
      Replace 'yourvenv' with the name of your choice.
      To activate your virtual environment use the command
         source yourvenv/Scripts/activate
      To deactivate type deactivate and press enter.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   Here's a simple Python program that prints "Hello, World!" to the console:
      print("Hello, World!")
   In this program, print is a function in Python that outputs text to the console. The text to be printed is provided as an argument within parentheses and must be enclosed in quotation marks, either single (') or double ("). This basic syntax includes the function name followed by parentheses containing the string argument, demonstrating Python's straightforward and readable code structure.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Integer (int): Represents whole numbers without a fractional part, e.g., 42, -7.
      # Integer
      age = 25
      print("Age:", age)

   Float (float): Represents numbers with a decimal point, e.g., 3.14, -0.001.
      # Float
      pi = 3.14159
      print("Pi:", pi)

   String (str): Represents a sequence of characters enclosed in single or double quotes, e.g., "Hello", 'World'.
      # String
      greeting = "Hello, World!"
      print("Greeting:", greeting)

   Boolean (bool): Represents logical values, either True or False.
      # Boolean
      is_student = True
      print("Is student:", is_student)

   List (list): Represents an ordered collection of items, which can be of different types, e.g., [1, 2, 3], ['a', 'b', 'c'].
      # List
      fruits = ["apple", "banana", "cherry"]
      print("Fruits:", fruits)

   Tuple (tuple): Similar to a list but immutable, e.g., (1, 2, 3), ('a', 'b', 'c').
      # Tuple
      coordinates = (10.0, 20.0)
      print("Coordinates:", coordinates)

   Dictionary (dict): Represents a collection of key-value pairs, e.g., {'name': 'Alice', 'age': 25}.
      # Dictionary
      person = {"name": "Alice", "age": 25}
      print("Person:", person)

   Set (set): Represents an unordered collection of unique items, e.g., {1, 2, 3}, {'a', 'b', 'c'}.
      # Set
      unique_numbers = {1, 2, 3, 2, 1}
      print("Unique numbers:", unique_numbers)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements are used to perform different actions based on different conditions. The most common conditional statements in Python are if, elif, and else.
   An example of basic use of 'if-else' statement is:

      age = 18

      if age < 18:
         print("You are a minor.")
      elif age == 18:
         print("You are exactly 18 years old.")
      else:
         print("You are an adult.")

   Loops are used to execute a block of code repeatedly. Python supports for and while loops.
   An example of basic use of 'for' loop is:

      fruits = ["apple", "banana", "cherry"]

      for fruit in fruits:
       print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are reusable blocks of code that perform a specific task. They allow you to organize your code into modular and manageable sections, making it easier to read, maintain, and debug.
   Below is a python function that takes two arguments and returns their sum:
      def add_numbers(a, b):
         return a + b

   To call this function:
      result = add_numbers(3, 5)
         print("The sum is:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Differences between lists and dictionaries:
      Lists are Ordered collections of items that are accessed by their index positions (starting from 0), while Dictionaries are Unordered collections of key-value pairs where each value is accessed using a unique key.

      Lists Can contain elements of any data type, including other lists, whereas in Dictionaries Keys must be immutable types (like strings, numbers, or tuples), but values can be of any data type.

      The script:
      
      numbers = [1, 2, 3, 4, 5]


      print("Original list:", numbers)
      numbers.append(6)  # Adding an element
      print("List after appending 6:", numbers)
      numbers[2] = 10  # Modifying an element
      print("List after modifying the third element:", numbers)
      removed_number = numbers.pop(1)  # Removing an element
      print("List after removing the second element:", numbers)
      print("Removed number:", removed_number)


      person = {
         "name": "Alice",
         "age": 30,
         "city": "New York"
      }


      print("Original dictionary:", person)
      person["email"] = "alice@example.com"  
      print("Dictionary after adding email:", person)
      person["age"] = 31 
      print("Dictionary after updating age:", person)
      removed_value = person.pop("city")  
      print("Dictionary after removing city:", person)
      print("Removed value:", removed_value)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python is a way to manage errors that may occur during the execution of a program. It allows you to handle these errors gracefully without crashing the program.
      try Block: Contains the code that might throw an exception.
      except Block: Catches and handles the exception if one occurs in the try block.
      finally Block: Contains code that will run regardless of whether an exception occurred or not. It is often used for cleanup actions.

      def divide_numbers(a, b):
          try:
             result = a / b
          except ZeroDivisionError as e:
             print("Error: Cannot divide by zero.")
             result = None
          except TypeError as e:
             print("Error: Both arguments must be numbers.")
             result = None
          else:
             print("Division successful.")
          finally:
             print("Execution of try-except block complete.")
          return result    

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   A module is a file containing Python code (functions, classes, variables) that can be imported and used in other Python scripts.

   A package is a collection of related modules stored in a directory. It often contains a special __init__.py file, which can be empty or execute initialization code for the package.

   TO import the entire math module:
      import math

   Using a function from the math module
      result_sqrt = math.sqrt(16)  # Calculates the square root of 16
      print("Square root of 16 is:", result_sqrt)

   Using a constant from the math module
      pi_value = math.pi
      print("Value of pi is:", pi_value)

   Importing specific functions from the math module
      from math import factorial, pow

   Using the imported functions
      result_factorial = factorial(5)  # Calculates 5!
      result_pow = pow(2, 3)  # Calculates 2 raised to the power of 3

      print("Factorial of 5 is:", result_factorial)
      print("2 raised to the power of 3 is:", result_pow)

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

   To read from a file in Python:
      Open the File: Use the open() function with the file path and mode ('r' for reading) to open the file.

      Close the File: Always close the file using the close() method to free up system resources.

   To make a script that reads the content of a file and prints it to the console:
      Define the file path
         file_path = 'sample.txt'

      Open the file for reading
      try:
         with open(file_path, 'r') as file:
      Read the entire content of the file
         content = file.read()
      Print the content to the console
         print("Content of the file:")
         print(content)
      except FileNotFoundError:
         print(f"Error: The file '{file_path}' does not    exist.")
      except IOError:
         print(f"Error: Unable to read the file '{file_path}'.")

   To write a list of strings to a file:
      Define the file path for writing
         file_path_write = 'output.txt'

   List of strings to write to the file
      lines_to_write = [
         "Hello, World!",
         "This is line 2.",
         "And this is line 3."
      ]

   Open the file for writing
   try:
         with open(file_path_write, 'w') as file:
   Write each line from the list to the file
         for line in lines_to_write:
            file.write(line + '\n')
         print(f"Data successfully written to '{file_path_write}'.")
   except IOError:
         print(f"Error: Unable to write to the file '{file_path_write}'.")


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


