# Python

In these so called "feynman techniqued note files" I will try to explain subjects, concepts, and much more in a very simple language that a 6 year old will be able to understand what is going on. Simple as in both it will be very elementary in english since it is not my native langage and simple because that is how the feynman technique works. Plus, since most of the programming concepts are extremly abstract I will try to give example analgoies from the real world, so that the reader will have easy time grasping the idea.

So with the neccessary greetings out of the way, let's look at what concept we are going to look at today; "PYTHON" is the name of it ... Basically we are going to learn what programming languages are and how compiled vs. interpreted programming languages differ from each other. Don't wory about the technical jargon yet, I will simplyfy all of them as we go along. And once those little concepts above are explained we can easily dive deep into what python is, how can we use python to write very good computer programs or just learn it for the fun of it.

Table of Contents:
- [Introduction](#introduction)
- [What is a Programming Language](#what-is-a-programming-language)
- [Difference between Interpreted vs Compiled](#difference-between-interpreted-vs-compiled)
- [Introduction to Python](#introduction-to-python)
  - [Getting Started](#getting-started)
  - [Operators](#operators)
  - [Data Types](#data-types)
  - [Control Flow](#control-flow)
  - [Functions](#functions)
  - [Classes](#classes)
  - [Input/Output](#input-output)
  - [Modules](#modules)
  - [Errors and Exceptions](#errors-and-exceptions)
  - [Files](#files)
  - [Additions](#additions)
  - [Little tour of Standart Libraries](#little-tour-of-standart-libraries)
  
# Introduction

So before we dive into the nitty-gritty details of what python is I wanted to say that not everything will be covered in this note file. As I said numeourus times above, this is just a feynman-styled-note-fite so it is meant to be kept short, neat and easy to understand by design. So if you are wondering the pythons lexers and parsers grammatical information (advanced topics, no need to worry) you are reading the wrong text. 

I will explain just the idea behind the concepts such as functions, classes, module imports ... etc. You wont see the advanced usage of them. This text is meant for the logic behind all of the ideas above. So with that out of the way! Lets get started.

# What is a Programming Language

`Python` is a "programming language", you may be wondering what is a "programming language" ? Well every person, animal ... etc. in this world communicates with each other through verbal expressions, signals and .. etc. the human-and-the-computer is no different. If we want to talk to computer we need a common ground where we can both understand each other, that is where programming languages comes into play .A programming language is essentially a software program that lets you speak to the computers hardware. Yes, the example I gave right now is **extremly** high-level and abstracted away from the details of what a programming language is ... However If I got into explaning what really is a programming language I would have to explain compilers too and I will do that in the `compilers` feynman-note.

So, the theory behind programming languages are really not that important when it comes to learning `python` and it is beyond the scope of this note file. Just know that a programming language is a software application(program) that you install to your computer that lets you talk to the computer's harware, and make the computer do what you want it to do. 

However, programming languages are really different than your usual day-to-day speaking language. Yes they both have grammar, syntax rules, vocabulary to construct expressions, sentences ... etc. But the computer does not think like the human brain. It is extremly primitive and "stupid" to be honest for such a smart device. While communicating you will have to tell the computer step by step about what to do and what you want it to do. So the language is a bit of a one-way-communication channel where you will be constantly telling computer to what to do and it just doing it without returning you any verbal expression unless you want it.

- `High-Level Programming Languages` -- Python is called a "high level" programming lanugage. You may be wondering what is that. High level basically means that the programming language is abstracted away from most of the concepts that is required to learn to write in lower level programming languages. For example without knowing how the computers work you cannot write good C code (a low level programming lanugage) yes you may code something nice and working but If you really want to use the language to its limits you need to understand how the computer works. But we do not have that problem with `python` since it is high level it is abstracted from most of the things regarding the underlying computer hardware. That does not mean that we do not need to know how computers work but essentially it makes our job easier. 

# Difference between Interpreted vs. Compiled

So now that we learned what computer programs are, now we can learn the different types of programming languages. There are two major ones really `interpreted` and `compiled`. Compiled languages like Java, C/C++ does not immideatly run your program. First you compile your program and the compiler outputs a "machine-code" (the code readable by your computer) and you run that code. So the protocol for using a compiled language is:
  ```
  write program -> compile it -> get the output file -> run that output file
  ```
  But python does not want this many steps while running a program. So they are what we call a interpreted language. They do not need to compile the code and run the outputted file. The interpreter does that for you, so you just write your program and than run that program with the interpreter:
  ```
  write program -> run the program
  ```
  easy piesy right

# Introduction to Python

We now that we have learned what are programming languages are or what are the differences between a compiled and a interpreted languages are let's now learn about what exactly is `python`. I do not need to repeat that python is a interpreted programming language you already know that. What I will tell you is that why is python designed in the way it is designed. So esentially to quote the man (Guido van Rossum) who created python itself *"Computer Programming for Everybody", in which he further defined his goals for Python: An easy and intuitive language just as powerful as major competitors. Open source, so anyone can contribute to its development.* That quote and design mentality has been the corner stone for every update python received. 

The language is kept extremly simple so that anybody can read or write in it without having to read hours of material. You can basically learn the basics of it over a weekend. And as it is mentioned above python is "open source" which means it is completly free and accepts contributions of work from everybody around the globe. 

# Getting Started

Before we dive into python's syntax rules and such ... we first need to install it into our computer. You can install it from [the official python.org](https://www.python.org/) or if you are familiar with the command line (terminal). You can install it with the following commands:
```
# for Ubuntu
$ sudo apt-get update
$ sudo apt-get install python3.6

# for Mac
brew install python
```

Now that we have installed it for testing purposes to see that the program is working correctly we are going to test it with a simple code. First go to your desktop or wherever you would like to create a new empty blank file. Name the file `test.py` (all python files created should have a .py extension.) and type the following inside the file and save it:
```python
print("Hello, World!")
```
Well for the final part let's learn how to run your python programs on your computer. Open up your command line (terminal) and once you change your directory to the `test.py` file's location (if you are not familiar with terminal, command line tools - read my shell feynman notes). And once you find that file you will need to use python's interpreter tool to run your `test.py` file. And to use it you just simply type python. Let's see an exmaple:
```
$ python test.py
```
The command above in the terminal outputs the following:
```
Hello, World!
```

# Comments

Before we get into how to write comments in python. Let's first understand what are comments and how are comments used inside a programming language. As it turns out writing code is not that hard but writing maintainable code that can be understood by many people ranging from different skillsets in the future is a very hard task. Believe it or not you usually won't even remember what code you wrote 2 days ago. That is why the founders of programming languages included a system called `comments`

Basically comments are lines of text that is included in some parts of the code so that the humans will have a better time understanding what is going on. They are kind of a sticky notes for the person who is maintaining, or writing that piece of code. Comments do not get executed by the interpreter at the runtime, they are simply there for the maintiner not for the final output of the program. And each language has their own form of snytax when it comes to writing comments. Let's see how python does it:
```python
# this is a single line comment, usaully added if the comment should be small
```
as you can see above if you start by writing `#` the right side of that text converts itself to a comment. It is best used for small comments. If you would like to write comments that spans more than couple of lines your best way of writing them is this:
```python
'''
This is a 
multi line comment
and this comment will
not get executed
by the interpreter :)
'''
```

# Variables

Now that we know how to write comments and run our code inside a terminal it is time to start learning the actual snyntax rules and logic of programming languages to implement some powerful code. Let's start with `variables`. Before we show it how to write it in python, let's first explore the logic behind it. So basically variables are "bags that contain information" what that means is that you can store data inside a container which you can access later on in your code. Lets see a basic exmaple first:
```python
# this is not python code it is psuedo-code

variable foo = 1
variable bar = 5

foo + bar  # outputs 6
```
As you have seen above variables are just containers that hold a value. The value can be a number, text, decimal pointed number, ... etc. (we will see what kind of data types you can put inside variables in the following chapters). And you need to give a name to your variables so that you can access them later on, in the above example we have two variables named `foo` and `bar`. By the way the `=` operator does not mean "equals to". In programming "equals to" have a different operator (`==`) a single `=` operator means that the data in the right side of that operator will be connected (assigned) to the left side of that operator.

Now that the logic is out of the way lets see how to write variables in python. Unlike other programminglanguages, python has no command for declaring a variable, you just give it a name and a variable is created the momoent you first assign a value to it:
```python
x = 10
y = "john doe"
print(x)
print(y)
```
The code above outputs:
```
10
john doe
```
Also you can change the variables value at any time you want:
```
x = 10
x = 555
print(x)  # prints 555
```

Now that we have seen the basics of now let's see some details that we can use for the curious readers. First variable names have rules:
  - You cant start a variable name with a number `2bar = 1` it is illegal and you will get an error.
  - You cant have a dash in between `foo-bar = 1` this is also illegal
  - You cant spaces in a name `foo bar = 1` this is also illegal
  
And lastly you can declare more than one variable inside a single code line like this:
```python
x, y, z = 1, 2, 3

print(x)  # 1
print(y)  # 2
print(z)  # 3
```
or you can simply give all of the variables the same value:
```python
x = y = z = 15
```

# Operators

Now that we know how to store some data inside variables, lets learn how we can do some operations on those data. We do not need to know most of the data types at the moment. We will just use numbers and string (text) data types for our variables. But most of the operations seen in this section can be used on all of the data types and after you learn the rest of the data types you can use the information here.

First I will give out a simple python exmaple of what we can do with various operators. However it would take too long to give out exmaples of each operator. Instead after a basic explanation I will just give every operator inside a grouped table:
```python
# basic operator usage

x = 10
y = 2

x + y   # 12
x - y   # 8
x ** y  # 100
x / y   # 5
```
When you operate on variables the operator does not change the data of the variables to the newly created (calculated) value. If you want to store the newly created value you need to store it on a  new array such as this:
```python
x, y = 10, 5
 
foo = x + y  # 15
```

Python divides the operators in the following groups:
  - Arithmetic operators
  - Assignment operators
  - Comparison operators
  - Logical operators
  - Identity operators
  - Membership operators
  - Bitwise operators
  
  > Do not worry if the operators below do not make sense yet. It will once you move to control flows. Just skim thorugh it and use it as a reference point.
  
Arithemtic Operators

| Operator | Name | Example |
| --|--|--|
| + | Addition | x + y |
| - | Subtraction | x - y |
| * | Multiplication | x * y |
| / | Division | x / y |
| % | Modulus | x % y |
| ** | Exponentation | x ** y |
| // | Floor Division | x // y |

Assignment Operators:
| Operator | Example | Same As |
| -- | -- | --|
| = | x = 5 | x = 5 |
| += | x += 3 | x = x + 3 |
| -= | x -= 3 | x = x - 3 |
| * = | x *= 3 | x = x * 3 |
| /= | x /= 3 |  x = x / 3 |
| %= | x %= 3 | x = x % 3 |
| //= | x //= 3 | x = x // 3 |
| **= | x **= 3 | x = x ** 3 |

> skipped: &= , |= , ^= , >>= , <<=

Comparison Operators:
|Operator | Name | Example | 
| --- | --- | --- |
| == | Equal | x == y |
| != | Not equal | x != y |
| > | Greater than | x > y |
| < | Less than | x < y |
| >= | Greater than or equal to | x >= y |
| <= | Less than or equal to | x <= y |

Logical Operators:
| Operator | Description | Example | 
| -- | -- | -- |
| and | Returns True if both statements are true | x < 5 and x < 10 | 
| or | Returns True if one of the statements is true | x < 5 or x < 4 |
| not | 	Reverse the result, returns False if the result is true | not(x < 5 and x < 10) | 

Identity Operators:
| Operator | Description | Example | 
| -- | -- | -- |
| is | Returns True if both variables are the same object | x is y |
| is not | Returns True if both variables are not the same object | x is not y |

Membership Operators:
| Operator | Description | Example | 
| -- | -- | -- |
| in | Returns True if a sequence with the specified value is present in the object | x in y |
| not int | Returns True if a sequence with the specified value is not present in the object | x not in y |

I am going to skip pythons Bitwise operators since it is not used on a day-to-day basis. It is usually used for special cases and if you are at that point why the hell are you reading this. 

# Data Types

Now lets understand what are the different data types we can assign to our variables. In the above chapters we have only used two data types `integers` (numbers) and `strings` (text inside ''). You have to understand that there are many more data types that called `primitive data types` of a language. Every language implements their own primitive data types and they differ from one language to another. Lets first see what kind of data types we can use and I will give specific examples and information for each one:
  - Text Type: `str` 
  - Numeric Types: `int`, `float`, `complex`
  - Sequence Types: `list`, `tuple`, `range`
  - Mapping Type: `dict`
  - Set Types: `set`, `frozenset`
  - Boolean Type: `bool`
  - Binary Types: `bytes`, `bytearray`, `memoryview`
  
By the way in case you are unsure of a variables data type you can use this built in tool of python within your code:
```python
x = 5
print(type(x))  # outputs <class 'int'>
```

### Text Type

### Numeric Types

### Sequence Types

### Mapping Type

### Set Types

### Boolean Type

### Binary Types

# Control Flow

# Functions

# Classes

# Input/Output

# Modules

# Errors and Exceptions

# Files

# Additions

# Little tour of Standart Libraries
