# Java Programming Fundamentals

## Introduction to Java Programming
- widely used, high-level programming lang originally developed by Sun Microsystems and maintanied by Oracle.
- platform independent, runs on Java Virtual Machine installed. Popular for appas and web services.

## Basic Syntax
- follows a similar syntax to C and C++. Designed tobe more readable and easier.
- basic syntax rules:
i) programs are organized into classes, must at least have 1 class.
ii) statements ended in semicolon
iii) case sensitive language

## Variable and Data Types
- variables used to store and manipulate data. Some commone data types:
i) int - used to store whole numbers
ii) double - used to store decimal numbers with more precision
iii) boolean - store values representing true or false
iv) string - store sequences of characters

## Control Flow
- refers to the order in which statements in a program are executed. Some common control flow statements:
i) if statement - used to execute block of code only if condition is true
ii) for loop - execute block of code repeatedly for a specific number of times
iii) while loop - used to execute code repeatedly as long as certain condition is true

## Object-Oriented Programming (OOP)
- relies heavily on the concept of objects and classes. Objects are instances (blueprints) of classes, defining properties and behaviours of objects.
- Java supports the following OOP principles:
i) Encapsulation - act of encapsulating data and methods within a class
ii) Inheritance - the abilty to create new classes based on existing ones.
iii) Polymorphism - the ability to use a single interface to represent different objects.

## Exception Handling
- exceptions are unexpected events occuring during execution of a program.
- prevents program from terminating abnormally.
- try-catch-finally blocks are used to handle exceptions.

## File Input and Output 
- classes and methods allow programmers to read from and write files.
- these are useful when dealing with large sets of data or when storing and retrieving information from external sources.
- e.g. of I\O operations in  Java are File, Scanner and PrintWriter

# Variables and Data Types

## Introduction
-variables are used to store and manipulate data. A variable acts a container holding a value of any data type.
-variables are declared before being used;several data types for diff purposes.

## Primitive Data Types
- Java has 8 primitive data types
- These data types are:
1) byte: a data type ranging from -128 to 127. Saves memory in large arrays where memory savings are important.
2) short: a data type ranging from -32,768 to 32,767. Saves memory in arrays when dealing with graphical data.
3) int: a data type storing whole numbers ranging from -2,147,483,648 to 2,147,483,647
4) long: s a data type that can store larger whole numbers ranging from
-9,223,372,036,854,775,808 to 9,223,372,036,854,775,807. It is often used when
dealing with very large numbers.
5) float: a data type that can store fractional numbers ranging from 3.4e^-038
to 3.4e^+038. It is mostly used for scientific calculations and situations that require a
large range of values.
6) double:  a data type that can store fractional numbers with a larger range
and precision than float. It can hold values from 1.7e^-308 to 1.7e^+308 and is the
default choice for decimal values.
7) char: a data type representing a single characters stores any Unicode character.
8) boolean: a data type representing true or flase values.

## Reference Data Types
- these data types are created using predefined classes or user defined classes
- commonly used are:
1) String: a sequence of characters used to store and manipulate text.
2) Arrays: ordered collection of elements of the same data type. Stores multiple values under a single variable name.
3) Classes: they define objects'properties and behaviour, they provide a way to represent real-world entities.

# Declaring and Initializing Variables
- variable must be declared with a specific data type, name and data type must be declared. e.g. int count;
- variables can be assigned a value e.g. int score = 100;
- variables can be assigned new values later in the program using the assignment opperator (=).

# Variable Naming Rules and Conventions
- names mus start with a leter, dollar sign or underscore.
- names can consist of letters, digits, dollar signs and underscores.
- variables are case sensisitve
- variables should be descriptive not lengthy
- use camel case for multi-word variable names

# Type Conversion
- Java provides automatic type conversion, typecasting, to handle diff data types'interactions.
- Implicit Casting: occurs when a smaller data type is assigned to a larger data type e.g. int num = 100;
double decimal = num;
- Explicit Casting: larger data type is assigned to a smaller data type, requires manual casting prevent data loss or overflow e.g. double decimal = 3.14;
int num = (int) decimal;

# Control Flow and Decision Making
## Introduction
- control flow refere to order which statements are executed in a program.
- allows control of flow of execution and direct program to perform specific actions based on certain conditions.

## If Statement
- the simplest form of a conditional statement. Allows program to execute block of code if specific condition is met.
## If-else Statement
- provides an alternative bloc of code to be executed if condition in the staement is not satisfied.
- allows program to take diff paths depending on whether the condition is true or false.

## Switch Statement
- allows program to select one of many code blocks to be executed based on the value of a variable or expression.
- useful when there are multiple possible cases to consider.

## Looping Statements
- allow programmers to repeat a block of code multiple times a specified condition is met.
- three main types of looping:
- While Loop: repeatedly executes a block of code as long as a certain condition is true. Commonly used when number of iterations is unkown.
- Do-while Loop: executes block of code repeatedly as long as a specific condition is true. Guarantees at least one execution of the code block as condition is check after code is executed.
- For Loop: executes a block of code a specific number of times. Provides control over loop parameters by intializing a variiable, specifiying condition and updating variable in a single line.