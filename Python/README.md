# Python
## Introduction to Python
1. Introduction 
### How Computers Work
- Computer memory is a grid where it stores files and data.
- A file with a file name is represented in the computer's directory.
- Along with file name is info stored about the file e.g. size.
- Access to contents of file, computer follows a pointer, an address representing location of file contents in memory.
- Writing and running a program is interaction with the memory.
- Programs generate bits of data (variables)- mini files.
- When assigning variable of the same data type in an array, they both point to the same location.
- This is working with the pc memory, inputting, retrieving and manipulating data. 

### Zen of Python
- Python is elegant fitting in modern era; e.g. syntax used to call one function is likely to be similar to that used to call a similar function.
- Python's true potential recognized in situations with complexities.
- Python's hidden mission statement "import this", drives this point home.

2. Getting Started with Python
### Variables and Types
- basic unit of a program is a variable, which is assigned a value.
- variable name cannot start with a number, can include upper and lower case letters including underscores.
- traditionally begin with lowercase
- several data types: intergers, floats, complex numbers, strings and booleans
- data structures allow for storage of a list of values in a single variable. 
- list: contains any data type, length of list determined by function. 
- set: similar to list, contains unique elements and declares using curly braces.
- order of elements in a set not important unlike list.
- Tuples: similar to lists, cannot be modified once declared. Useful storing large amounts of data in memory.
- Dictionary: a collection of key-value pairs, similar to a word and it's definition.

### Operators
- instructions that perform operations on variables and values.
- manipulate and perform action on data. (e.g arithmetic operator)
- Logical operators: 'and', 'or' and 'not' operating on Boolean values.
- Membership operators: 'in' and 'not in' used to check whether a value is present in a sequence or not.

### Control Flow
- if statment: allows to execute a block of code only if a certain condition is met. Used to iterate over a list or object.
- for loop: a variable representing current item in list
- while loop: loops until a certain condition is false.

### Functions
- like a machine that takes inputs and produces ouputs
- functions in python are defined by 'def' keyword followed by function name
- 'return' keyword is used to specify the output.
- functions can take one or more arugments, may or may not return a value.

### Classes and Objects
- Classes contain multiplr functions and attributes; it is defined by an uppercase letter.
- Usually begin by creating the 'init' function, which gets called eveyrtime an instance of a class is created.
- We can acces any of the attributes or functions in the class using 'self' variable.

### Ints and Floats
- Python automatically returns a float to accommodate non-whole numbers. Adding a float to an int or multiplying or using exponents with both also returns a float. 
- Casting: when we convert from one type to another, such as float to int.
- One pitfall of floats is that they are approximations, which can result in rounding errors

### Alternative Number Types
- passing numbers as strings, int class converts it to integer
- decimal: addresses some of the issues we have with floats; need to import decimal class and the getcontext function
- with decimal, we can instantiate a decimal object with a number value.
- Booleans; 1 is true and 0 is false; with strings true is true.
- Data structures can also be casted to booleans.

### Strings
- Slicing: analyzes and constructs strings, taking a portion of a string and returning it.
- F-strings: allow us to insert variables or expressions inside curly braces in a string. 
- Rounding and number formatting can be done with F-strings.
- Multi-line strings: use tripple quotes; to include literal triple quotes in string, can escpe with backslash.

### Bytes
- a sequence of data that is in a form of raw data in a form of ones and zeros.
- commonly used for streaming files or transmitting texts without knowing the encoding.
- bytes objects are immutable, like tuples, but you can use a byte array if you need to modify the data. 

### Lists
- slicing can also be used in lists to extract a range of values, can also add a third value to control step size.
- range function used to generate longer lists, also sliced.
- negative values can be used to step backward through the list. 
- adding in a list = append() method
- insert at specific position = insert() method 
- removing items from a list = remove() [removes based on value not index] or pop() [end of the list] method
- a loop with pop() can be used to remove all items from list.
- make a copy of a list so that changes to one list don't affect the other = copy () method

### Tuples and Sets
- set: defined using curly brackets e.g. {},mySet or mySet = set(('a', 'b','c')) 
- set removes duplicates from a list, since sets only contain unique values. 
- can check if element is in a set using membership operator (in) and find lenght of set using length() function.
- tuples: declared with parentheses instead of square
- tuples are immutable, can retrieve elements from tuple using indexing
- tuples take up less memory
- common use case is when you want to return multiple values from a function

### Dictionaries 
- to access a specific key-value pair in the dictionary, simply type name of dictionary followed by key in square brackets
- to add new key-value pair, use a similar syntax with assigment operator
- you can also access keys and values of a dictionary using .keys() and .values() methods.
- len() function to get length of dictionary

### List Comprehensions
- refers to comprehensive listing of things
- using a list comprehension you can multiple each item in the list by two e.g. two times item in my list
- allows us to create a for loop in one line while returning a copy of the list you're iterating over.
- also endables filtering or applying functions to every item

### Dictionaries and Comprehensions 
- in python dictionary comprehensions to create new dicitonary from an iterable structure, similar to list comprehensions
- to turn dictionary back into list, use 'items' method returning 'dict_items' object with key-value pairs
-  use a list comprehension with the syntax "name_value = [{'name': key, 'value': value} for key, value in animals.items()]" to create a list of dictionary objects with the original keys and values under the "name" and "value" fields

### If and Else
- this statement evaluates a series of values and runs the code instructions corresponding to the first true value found.
- elif statement, used to write clean and readable code
- rule is to write a single if statement followed by any number of elif statments, optionally a single else statement at the very end to provide default value if nothing matches.

### While 
- while loops can run forever if not exited using a break statement, which moves on to the next line of code outside the loop.
- if you want to skip over certain lines within a loop, you can use continue statement, which skips over any lines after it and jumps back to the top of the loop.

### For
- a new variable is declared to hold the value of each element in list as you iterate through it.
- you can also use pass, continue and break
- break else statement is used to find prime numbers in a few lines of Python
- break else can also be used in while loops, this statement makes your code look clean

## Python Fundamentals
### Basic Functions
- a basic unit of a program is not code but a function, it gives a program functionality.
- they are composed of a name and parameters, denoted by a def statement.
- parameters are passed on as arguments in functions, own values can be assigned to specific needs.
- when calling the function, pass in the message before or after the operation, as long as we specify which argument is which by using a comma to separate them.
- args = they come after the positional arguments, order of first two arguments is important and can't be changed.
- there is functional limitation to how many variables can be anticipated.
- kwargs = handles any keyword arguments; have keys and values and can be passed in any order, dictionary more appropriate data structure for referencing them.

### Variables and Scope 
- function scope = locals function, allows us to access all the variables within a python function
- variable names that are only accessible locally within the function. 
- globals = built-in function that returns a dictionary representing the current global symbol table.

### Functions As Variables
- for functions, data includes information about required parameters and the lines of instruction to be executed. In Python, a function is represented as an object
- the "code" attribute of Python function objects can be used to confirm that functions are just variables in Python
-  there are two text processing operations, and a function that can make the text lowercase, remove punctuation, new lines, and words that are three characters or less. It can also remove long words. By calling these functions in a list, the order can be changed or decide which functions to apply. 
- lambda functions = a function without giving it a variable name. Just like how an expression like 5 or 2 + 3 can be written without assigning it to a variable, a small function can be defined using the lambda keyword

### Anatomy of a Class
- Instance Attributes = attributes that every instance of a class can possess; it makes it easier for creating new instances
- Static Attributes = defined outside the constructor, each instance of class will have the same value of argument; attribute can be accessed directly on class itself
- they are static as they don't change with each instance and commonly used to hold constants or business logic.

- getter method = retrieves value of variable; no need to pass self attribute for method; call method in traditional way but can also call it with self.

### Instance and Static Methods
- clean text method = a static method as it does not belong to any particular class instance; use class name or class instance to refer to static variables
- add text method = an instance method belonging to a particular class instance

### Class Inheritance
- it is possible for one class to inherit all the methods and attributes of another class. The original class is referred to as the parent class, while the new class that extends it is known as the child class. This inheritance process happens automatically when the child class is created. 

- we can also apply class extensions in Python's built-in classes. In Python, creating a new list can be done by instantiating it as "list". Although it appears as a function, "list" is actually a class