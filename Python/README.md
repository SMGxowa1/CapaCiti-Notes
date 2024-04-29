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
## Variables and Types
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

## Operators
- instructions that perform operations on variables and values.
- manipulate and perform action on data. (e.g arithmetic operator)
- Logical operators: 'and', 'or' and 'not' operating on Boolean values.
- Membership operators: 'in' and 'not in' used to check whether a value is present in a sequence or not.

## Control Flow
- if statment: allows to execute a block of code only if a certain condition is met. Used to iterate over a list or object.
- for loop: a variable representing current item in list
- while loop: loops until a certain condition is false.

## Functions
- like a machine that takes inputs and produces ouputs
- functions in python are defined by 'def' keyword followed by function name
- 'return' keyword is used to specify the output.
- functions can take one or more arugments, may or may not return a value.

## Classes and Objects
- Classes contain multiplr functions and attributes; it is defined by an uppercase letter.
- Usually begin by creating the 'init' function, which gets called eveyrtime an instance of a class is created.
- We can acces any of the attributes or functions in the class using 'self' variable.

## Ints and Floats
- Python automatically returns a float to accommodate non-whole numbers. Adding a float to an int or multiplying or using exponents with both also returns a float. 
- Casting: when we convert from one type to another, such as float to int.
- One pitfall of floats is that they are approximations, which can result in rounding errors

## Alternative Number Types
- passing numbers as strings, int class converts it to integer
- decimal: addresses some of the issues we have with floats; need to import decimal class and the getcontext function
- with decimal, we can instantiate a decimal object with a number value.
- Booleans; 1 is true and 0 is false; with strings true is true.
- Data structures can also be casted to booleans.

## Strings
- Slicing: analyzes and constructs strings, taking a portion of a string and returning it.
- F-strings: allow us to insert variables or expressions inside curly braces in a string. 
- Rounding and number formatting can be done with F-strings.
- Multi-line strings: use tripple quotes; to include literal triple quotes in string, can escpe with backslash.

## Bytes
- a sequence of data that is in a form of raw data in a form of ones and zeros.
- commonly used for streaming files or transmitting texts without knowing the encoding.
- bytes objects are immutable, like tuples, but you can use a byte array if you need to modify the data. 

## Lists
- slicing can also be used in lists to extract a range of values, can also add a third value to control step size.
- range function used to generate longer lists, also sliced.
- negative values can be used to step backward through the list. 
- adding in a list = append() method
- insert at specific position = insert() method 
- removing items from a list = remove() [removes based on value not index] or pop() [end of the list] method
- a loop with pop() can be used to remove all items from list.
- make a copy of a list so that changes to one list don't affect the other = copy () method

## Tuples and Sets
- set: defined using curly brackets e.g. {},mySet or mySet = set(('a', 'b','c')) 
- set removes duplicates from a list, since sets only contain unique values. 
- can check if element is in a set using membership operator (in) and find lenght of set using length() function.
- tuples: declared with parentheses instead of square




