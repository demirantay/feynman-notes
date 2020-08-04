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
  
## Introduction

So before we dive into the nitty-gritty details of what python is I wanted to say that not everything will be covered in this note file. As I said numeourus times above, this is just a feynman-styled-note-fite so it is meant to be kept short, neat and easy to understand by design. So if you are wondering the pythons lexers and parsers grammatical information (advanced topics, no need to worry) you are reading the wrong text. 

I will explain just the idea behind the concepts such as functions, classes, module imports ... etc. You wont see the advanced usage of them. This text is meant for the logic behind all of the ideas above. So with that out of the way! Lets get started.

## What is a Programming Language

`Python` is a "programming language", you may be wondering what is a "programming language" ? Well every person, animal ... etc. in this world communicates with each other through verbal expressions, signals and .. etc. the human-and-the-computer is no different. If we want to talk to computer we need a common ground where we can both understand each other, that is where programming languages comes into play .A programming language is essentially a software program that lets you speak to the computers hardware. Yes, the example I gave right now is **extremly** high-level and abstracted away from the details of what a programming language is ... However If I got into explaning what really is a programming language I would have to explain compilers too and I will do that in the `compilers` feynman-note.

So, the theory behind programming languages are really not that important when it comes to learning `python` and it is beyond the scope of this note file. Just know that a programming language is a software application(program) that you install to your computer that lets you talk to the computer's harware, and make the computer do what you want it to do. 

However, programming languages are really different than your usual day-to-day speaking language. Yes they both have grammar, syntax rules, vocabulary to construct expressions, sentences ... etc. But the computer does not think like the human brain. It is extremly primitive and "stupid" to be honest for such a smart device. While communicating you will have to tell the computer step by step about what to do and what you want it to do. So the language is a bit of a one-way-communication channel where you will be constantly telling computer to what to do and it just doing it without returning you any verbal expression unless you want it.

- `High-Level Programming Languages` -- Python is called a "high level" programming lanugage. You may be wondering what is that. High level basically means that the programming language is abstracted away from most of the concepts that is required to learn to write in lower level programming languages. For example without knowing how the computers work you cannot write good C code (a low level programming lanugage) yes you may code something nice and working but If you really want to use the language to its limits you need to understand how the computer works. But we do not have that problem with `python` since it is high level it is abstracted from most of the things regarding the underlying computer hardware. That does not mean that we do not need to know how computers work but essentially it makes our job easier. 

## Difference between Interpreted vs. Compiled

So now that we learned what computer programs are, now we can learn the different types of programming languages. There are two major ones really `interpreted` and `compiled`. Compiled languages like Java, C/C++ does not immideatly run your program. First you compile your program and the compiler outputs a "machine-code" (the code readable by your computer) and you run that code. So the protocol for using a compiled language is:
  ```
  write program -> compile it -> get the output file -> run that output file
  ```
  But python does not want this many steps while running a program. So they are what we call a interpreted language. They do not need to compile the code and run the outputted file. The interpreter does that for you, so you just write your program and than run that program with the interpreter:
  ```
  write program -> run the program
  ```
  easy piesy right

## Introduction to Python

We now that we have learned what are programming languages are or what are the differences between a compiled and a interpreted languages are let's now learn about what exactly is `python`. I do not need to repeat that python is a interpreted programming language you already know that. What I will tell you is that why is python designed in the way it is designed. So esentially to quote the man (Guido van Rossum) who created python itself *"Computer Programming for Everybody", in which he further defined his goals for Python: An easy and intuitive language just as powerful as major competitors. Open source, so anyone can contribute to its development.* That quote and design mentality has been the corner stone for every update python received. 

The language is kept extremly simple so that anybody can read or write in it without having to read hours of material. You can basically learn the basics of it over a weekend. And as it is mentioned above python is "open source" which means it is completly free and accepts contributions of work from everybody around the globe. 

## Getting Started

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

## Comments



## Data Types

## Operators

## Control Flow

## Functions

## Classes

## Input/Output

## Modules

## Errors and Exceptions

## Files

## Additions

## Little tour of Standart Libraries
