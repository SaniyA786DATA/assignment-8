Q.1. What are keywords in python? Using the keyword library, print all the python keywords.


Python Keywords: An Introduction
Value Keywords: True, False, None.
Operator Keywords: and, or, not, in, is.
Control Flow Keywords: if, elif, else.
Iteration Keywords: for, while, break, continue, else.
Structure Keywords: def, class, with, as, pass, lambda.
Returning Keywords: return, yield.
Import Keywords: import, from, as.

Q.2. What are the rules to create variables in python?

1. Variable names can only contain letters, numbers, and underscores: You can use letters (a-z, A-Z), numbers (0-9), and underscores (_) in your variable names.

2. Variable names cannot start with a number: You cannot start your variable name with a number, but you can use numbers in the middle or at the end.

3. Variable names cannot contain spaces: You cannot use spaces in your variable names. Instead, use underscores (_) to separate words.

4. Variable names cannot use Python's reserved words: You cannot use Python's reserved words (such as if, else, for, while, etc.) as variable names.

5. Variable names are case-sensitive: Variable names are case-sensitive, which means that "hello" and "Hello" are two different variables.

Examples:

valid_variable_name = "hello_world"
invalid_variable_name = "123hello"  // starts with a number
invalid_variable_name = "hello world"  // contains a space
invalid_variable_name = "if"  // is a reserved word


Q.3. What are the standards and conventions followed for the nomenclature of variables in
python to improve code readability and maintainability?

In Python, there are certain standards and conventions followed for the nomenclature of variables to improve code readability and maintainability. Here are some of them:

1. Use meaningful and descriptive names: Choose variable names that accurately describe the purpose and content of the variable. This helps other developers understand the code and makes it easier to maintain.

2. Use lowercase letters and underscores: Python's official style guide, PEP 8, recommends using lowercase letters and underscores to separate words. This makes the code more readable and easier to understand.

3. Avoid using single-letter variable names: Single-letter variable names can be confusing and make the code harder to understand. Instead, use descriptive names that indicate the variable's purpose.

4. Use consistent naming conventions: Use consistent naming conventions throughout the code. For example, if you're using underscores to separate words, use them consistently.

5. Avoid using reserved words: Avoid using Python's reserved words (such as if, else, for, while, etc.) as variable names. This can cause confusion and make the code harder to understand.

6. Use nouns for variable names: Use nouns for variable names to indicate that they hold values. For example, "user_name" is a better variable name than "getUser".

7. Use verbs for function names: Use verbs for function names to indicate that they perform actions. For example, "get_user_name" is a better function name than "userName".

8. Use plural nouns for lists: Use plural nouns for lists to indicate that they hold multiple values. For example, "user_names" is a better variable name than "userName".

9. Avoid using abbreviations: Avoid using abbreviations unless they're widely recognized and accepted. Instead, use descriptive names that accurately describe the variable's purpose.

10. Follow PEP 8 guidelines: PEP 8 is Python's official style guide, and it provides guidelines for coding style, syntax, and naming conventions. Following PEP 8 guidelines can help improve code readability and maintainability.

By following these standards and conventions, you can write more readable, maintainable, and efficient Python code.

Here are some examples of good and bad variable names:

Good variable names:

- user_name
- user_names
- get_user_name
- calculate_total

Bad variable names:

- x
- getUser
- tn
- calculateT

Q.4. What will happen if a keyword is used as a variable name?

In Python, if a keyword is used as a variable name, it will result in a SyntaxError.

Keywords are reserved words in Python that have special meanings and are used for specific purposes, such as:

- if, else, for, while, class, def, etc.

If you try to use a keyword as a variable name, Python will raise a SyntaxError because it will interpret the keyword as a statement or a syntax element, rather than a variable name.

Here's an example:

>>> if = 5
SyntaxError: invalid syntax

In this example, the keyword if is being used as a variable name, which is not allowed. Python raises a SyntaxError because it expects the if keyword to be used as a conditional statement, not as a variable name.

Similarly, if you try to use other keywords as variable names, you will get a SyntaxError:

>>> class = "hello"
SyntaxError: invalid syntax

>>> def = 10
SyntaxError: invalid syntax

To avoid this error, it's essential to choose variable names that are not keywords. You can use the keyword module in Python to check if a name is a keyword:

>>> import keyword
>>> keyword.iskeyword("if")
True
>>> keyword.iskeyword("hello")
False

So, always choose variable names that are descriptive, unique, and not keywords!

Q.5. For what purpose def keyword is used?

In Python, the def keyword is used to define a function.

A function is a block of code that can be executed multiple times from different parts of a program. Functions are useful for:

1. Modularizing code: Breaking down a large program into smaller, reusable pieces of code.
2. Reusing code: Avoiding duplicated code by defining a function that can be called multiple times.
3. Organizing code: Grouping related code together to make it easier to understand and maintain.

The def keyword is used to define a function by specifying its name, parameters, and body. The basic syntax is:

def function_name(parameters):
    # function body

Here's an example:

def greet(name):
    print("Hello, " + name + "!")

greet("John")  # Output: Hello, John!

In this example, the def keyword is used to define a function named greet that takes a single parameter name. The function body prints a personalized greeting message.

The def keyword is followed by the function name, which should be a valid Python identifier. The parameters are listed in parentheses, and the function body is indented under the def statement.

Functions can also return values using the return statement:

def add(x, y):
    return x + y

result = add(2, 3)
print(result)  # Output: 5

In summary, the def keyword is used to define a function in Python, which allows you to modularize, reuse, and organize your code.

Q.6. What is the operation of this special character ‘\’?

In Python, the special character \ is called the "backslash" or "escape character".

The backslash (\) has several operations:

1. Escape character: When used in a string, the backslash is used to escape special characters, such as:
    - \n: newline
    - \t: tab
    - \r: carriage return
    - \\: backslash itself
    - \': single quote
    - \": double quote

Example:

print("Hello\nWorld")  # Output: Hello
                       #         World

1. Line continuation: When used at the end of a line, the backslash indicates that the statement continues on the next line.

print("Hello, " + \
      "World")  # Output: Hello, World

1. Path separator: In Windows, the backslash is used as a path separator in file paths.

print("C:\Users\username\Documents")

1. Regular expressions: In regular expressions, the backslash is used to escape special characters or to indicate a special sequence.

import re
pattern = r"\d+"  # matches one or more digits

1. Raw strings: When used with the r prefix, the backslash indicates a raw string, where backslashes are treated as literal characters.

print(r"C:\Users\username\Documents")  # Output: C:\Users\username\Documents

In summary, the backslash (\) is a special character in Python that serves multiple purposes, including escaping special characters, line continuation, path separation, regular expressions, and raw strings.

Q.7. Give an example of the following conditions:
(i) Homogeneous list
(ii) Heterogeneous set
(iii) Homogeneous tuple

Here are the examples:

(i) Homogeneous list

A homogeneous list is a list that contains elements of the same data type.

Example:

fruits = ["apple", "banana", "cherry"]

In this example, the list fruits contains only strings, making it a homogeneous list.

(ii) Heterogeneous set

A heterogeneous set is a set that contains elements of different data types.

Example:

mixed_set = {1, "hello", 3.14, True}

In this example, the set mixed_set contains an integer (1), a string ("hello"), a float (3.14), and a boolean (True), making it a heterogeneous set.

(iii) Homogeneous tuple

A homogeneous tuple is a tuple that contains elements of the same data type.

Example:

numbers = (1, 2, 3, 4, 5)

In this example, the tuple numbers contains only integers, making it a homogeneous tuple.

Note that in Python, tuples are immutable, meaning their contents cannot be changed after creation.

Q.8. Explain the mutable and immutable data types with proper explanation & examples.

In Python, data types can be classified into two categories: mutable and immutable.

Immutable Data Types:

Immutable data types are those that cannot be changed or modified after they are created. Once an immutable object is created, its state cannot be altered.

Examples of immutable data types in Python:

1. Integers: Integers are whole numbers that cannot be changed after they are created.

a = 5
print(a)  # Output: 5
a = 10
print(a)  # Output: 10 (a new object is created)

In this example, the integer a is assigned a new value, but a new object is created, and the original object remains unchanged.

1. Floats: Floats are decimal numbers that cannot be changed after they are created.

a = 3.14
print(a)  # Output: 3.14
a = 2.71
print(a)  # Output: 2.71 (a new object is created)

1. Strings: Strings are sequences of characters that cannot be changed after they are created.

a = "hello"
print(a)  # Output: hello
a = "world"
print(a)  # Output: world (a new object is created)

1. Tuples: Tuples are ordered collections of objects that cannot be changed after they are created.

a = (1, 2, 3)
print(a)  # Output: (1, 2, 3)
a = (4, 5, 6)
print(a)  # Output: (4, 5, 6) (a new object is created)

Mutable Data Types:

Mutable data types are those that can be changed or modified after they are created. The state of a mutable object can be altered after it is created.

Examples of mutable data types in Python:

1. Lists: Lists are ordered collections of objects that can be changed after they are created.

a = [1, 2, 3]
print(a)  # Output: [1, 2, 3]
a.append(4)
print(a)  # Output: [1, 2, 3, 4] (the original object is modified)

1. Dictionaries: Dictionaries are unordered collections of key-value pairs that can be changed after they are created.

a = {"name": "John", "age": 30}
print(a)  # Output: {'name': 'John', 'age': 30}
a["city"] = "New York"
print(a)  # Output: {'name': 'John', 'age': 30, 'city': 'New York'} (the original object is modified)

1. Sets: Sets are unordered collections of unique objects that can be changed after they are created.

a = {1, 2, 3}
print(a)  # Output: {1, 2, 3}
a.add(4)
print(a)  # Output: {1, 2, 3, 4} (the original object is modified)

In summary, immutable data types cannot be changed after they are created, while mutable data types can be modified after they are created.

Q.9. Write a code to create the given structure using only for loop.
*
***
*****
*******
*********

Here is a Python code that creates the given structure using only a for loop:

for i in range(1, 6):
    print("* " * i)

This code uses a for loop to iterate from 1 to 5, and in each iteration, it prints a string of asterisks (*) followed by a space. The number of asterisks printed in each iteration increases by 1, creating the desired structure.

Here's the output:

* 
* * 
* * * 
* * * * 
* * * * * 

Note that I used the * operator to repeat the string "* " by the current value of i. This is a concise way to create the desired pattern.

Alternatively, you can use a for loop with a range of numbers to create the structure:

for i in range(1, 6):
    for j in range(i):
        print("*", end=" ")
    print()

This code uses a nested for loop to print the asterisks. The outer loop iterates from 1 to 5, and the inner loop iterates from 0 to i-1. In each iteration of the inner loop, it prints an asterisk followed by a space. The end parameter of the print function is set to " ", which means that the next print statement will continue on the same line. After the inner loop finishes, the outer loop prints a newline character to move to the next line.

Q.10. Write a code to create the given structure using while loop.
|||||||||
|||||||
|||||
|||
|

Here is a Python code that creates the given structure using a while loop:

i = 9
while i > 0:
    print("|" * i)
    i -= 1

This code uses a while loop to iterate from 9 to 1, and in each iteration, it prints a string of vertical bars (|) repeated i times. The value of i decreases by 1 in each iteration, creating the desired structure.

Here's the output:

|||||||||
|||||||||
|||||||
|||||
|||
||
|

Note that I used the * operator to repeat the string "|" by the current value of i. This is a concise way to create the desired pattern.

This code works as follows:

- Initially, i is set to 9.
- The while loop condition is i > 0, which means the loop will continue as long as i is greater than 0.
- In each iteration, the code prints a string of vertical bars (|) repeated i times using the expression "|" * i.
- After printing the string, the code decrements i by 1 using the statement i -= 1.
- The loop continues until i becomes 0, at which point the loop condition becomes false, and the loop exits.


```python

```


```python

```


```python

```
