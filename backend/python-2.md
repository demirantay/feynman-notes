# Control Flow

Again and again as you have guessed by now we always start by explaning what the concept is and then move on to writing it in a python syntax. Well control flow is used to control the logic in your code. How do you ask? simple, if I explain it with examples it will be way better and easier to understand. Do you remember the student grades code we have written in the first part? If so, lets build up on that example. We need to graduate the students but while doing that wee need to control the graduation flow with pass or fail status each student based on their grades. Simple right? You just control the logic of the code. 

Now that we have understood the logic behind the "control flow" lets get to learnign how to implement it in python syntax. Do you remember the the operators for expressions wuch as `>`, `<`, `==` ? So, we are going to use those operators to create an expression and check with `if`, `else`, `elif` keywords that are reserved by the python langauge just for the control flow:
```python
# Lets create our students

grades = {
  "luka": 95,
  "josie": 34
}

if grades["luka"] > 50:
    print("pass!")

if grades["luka"] < 50:
    print("fail")
```
as you have seen above if we ran the code it would output `pass!` since luka's grade is 95 and above 50. So what do we get out from the code snippet above? That if the `if` keywords is used python looks for the expression in it's right part and if that expression is `True` it executes the code block below. (You need 4 spaces to tell python that the codeblock is in that `if` is scope.

Now you may be wondering well wouldnt that take a lot of if statements inside the code if the data control logic is too much. And you would be right. We can simplyfy the above code with the following `else` keywords:
```python
if grades["luka"] > 50:
    print("pass")
else:
    print("fail")
```
What it does here that if the `if` keywords is NOT True than the `else` block gets executed. Now that it starts make sense we can include a new keyword to the mix `elif` its a mixture of both "else if" so the control flow will check the if block first if it is false than it will move on to the next `else if` block and once every keywords is false. It will than finally check the else statement.
```python
if grades["luka"] > 90:
    print("A")
elif grades["luka"] > 80:
    print("B")
elif grades["luka"] > 70:
    print("C")
elif grades["luka"] > 60:
    print("D")
else:
    print("F")
```
So now in the above code we have coded a new concept instead of just entering pass or fail. Now the code can decide what kind of grade you will receive based on the students grade. You may be asking "hold up! I could easily do all of this with just only `if` keywords" and you would be 100% right but remember the first thing I said in the begining of this note file. Readability and maintainability is waaay more important than just slapping some code into the file. Using all of the control flow statements and keywords help the code be more readable. 

# Loops

First lets talk about what loops are and how are they used in the code's logic. In computer science, a loop is a programming structure that repeats a sequence of instructions until a specific condition is met. Sounds a bit scary right? No its actually easy once you learn its logic so bascially think about those if blocks we defined above. `If` blocks code executres once a condition is met. In loops the code bloock executes repedeatly without stopping until a condition is met. This means that unless the condition is met the loop will run the code indefinetly. 

In python we have two ways of wrriting loops:
  - `while` statement.
  - `if` statement.

- Let's see an example of the `while` loops:
  ```python
  i = 1
  while i < 6:
      print(i)
      i += 1
  ```
  So in the above code the program will output numbers starting from 1, 2, ... to 5. Because everytime the loop executes the code at the end our variable `i` gets incremented by 1. And the condition of the loop is that the `i` should be less than 6. So as we have described above if the condition was wrong or by design did not have control mechanism it would go idfeinietly. Lets see indefenite loops:
  ```python
  i = 1
  while i > 0:
    print(i)
    i += 1
  ```
  This will create an indefinite loop because the condition and its control mechanism at the bottom do not stop the loop. Instead it feeds it. By the way if you want to create a indefinite loop by deisng you can simply use True boolea value:
  ```python
  while True:
      # execute
  ```
  
- Before we get into `for` loops we should talk about `control` statements of a loop. They can be used in for loop but they mostly go hand in hand with `while` loops. You use control statements to control the state of the loop. If the loop reach a certain value you can either skip that values repeat cycle or just simply break the loop. The two control statements for these operations are : `break`, `continue`. 
  ```python
  while True:
      foo = input(...)
      
      if foo == "stop":
          break
       if foo == "gibersih value":
          continue
  ```
  This loop above will continue to ask for user input unless the value is "stop". If it is stop than the break control statement will be executed and the loop will be terminated. 
  
- `for` loops -- are mostly used when you want to traverse a data sequence such as lists, tuples, distionaries ... etc.
  ```python
  fruits = ["apple", "banana", "cherry"]
  for x in fruits:
    print(x)
  ```
  
- If you are familiar with another language than you have used this type of for loop before:
  ```
  for (i=0; i<10; i++) { ... }
  ```
  If you haven't used this type of for loops before let me explain. So bascially like in whiel you define your i in the begining, and in the second control part checks if the condition is met. If the i is less then 10 then the code will execute. And the last part is like in the while loop it iterates the initial value so that the code will not go infitie. If you are wondering well this is exactly like while loop but in a different writing style then you would be exactly right. But in python you write this like this (dont worry nearly everyone fucking forgets this for loop syntax in python for some reason it is not that easy to remember)
  ```python
  for i in range(0, 10, 1):
      # loop code
  ```

# Functions

Again lets stat off by defining what functions are, and how they are used in the context of programming and than later on we will move on to learning how to write them in python. So, when you will write a fairly medium sized program or even a small one, you will never want to repeat yourself while writing a code. What do i mean is that for example see the below code in psuedo-code:
```
var a = 10
var b = 20

var sum1 = a + b

var c = 13
var d = 65

var sum2 = c + d
```
as you can the above code it is fairly simple. You are just trying to output the sum of 4 different variables grouped into two. However if we wrote a function, we could use the same formula such as `foo + foo` and would not have to define variables to be used in our sum variables. A picture is a thousand words, so let's see the following:
```
function sum(a + b) { 
    return a+b
}

summary_1 = sum(10, 20)
summary_2 = sum(13, 65)
```

...

# Classes

...

# Input/Output

First lets understand what input and output does in a computer program. So basically in it's name an input gets an input from the user. It might be a keyboard char, a mouse click .. etc. anything really that is provided from the user. And the output is what our computer outputs (shows) to the user. They are bascially a primitive communication line between a human and a computer. (yes, you can also output values to other programs and chain them but for the sake of simplicity i just menitoned humans and computers)

Lets see how they are used in python. Python uses `input()` function that comes with the standart library. For example if you want to get a user input and store it in it somewhere you use this:
```python
username = input("enter username:")
```
But input() always reutrns you a string. So how do you fix that problem and get other values ? Simple! you use conversion methods that we learned above:
```
teleophone = int(input("phone number: "))
```
as you can see in the aobve code we have converted the entered string number to a integer. 

And now lets see how we output stuff to the user or computer. By now you ahve seen it used number of times so you know how it operates:
```python
username = "foo"

print(username)
```
yes good old `print()` is used for printing and outputtung text to the users. Well, you may be wondering well what is there to learn about it and you would be suprised. But for now lets just see the basics of interestnig things we can do with print:
```
print("hello" + str(username) + " , nice to meet you!")
```
You can add variables inside a print statement so that the output dynamiacally changes based on the variables that are passed on to it. You can also format your print values with var.format() function. However these are beyond the scope of this file. Just know print() is your go to function for output. But if you want to dive deeper you can findout more output functions and methods.

# Modules

When you write programs that has more than 1000 lines of code it is a good idea to start moduling up your code base. What does using modules mean ? Well it is not concept solely meant for programmers. Modules are used in nearly every profession out there. It is basically used when the task is too giagantic you just break it up into smaller segments. and each segments get connected to make a larger piece. And each small segment is called modules. That is the same in programming. You cannot just jam all of your code into a single file . (Yes theoritallcy you can do it, but remember readability and maintainiabiltiy is waaaay more important than anything else) 

So it is a very good idea to break your code into logical modules and design them in a smart way that you will have no problems while plugging and connecting them with each other.

So how do we define and use modules in python ? By the way before we learn how to write modules snytaticaly in python. Lets take another look on how to structure them. Yes, there are exceptions but for the most of the time you should have an entry point to your program called `main.py` and this will be used to access to the rest of the modules. And each module should contain functions and classes. If you make your modules as libraries you simply just have to control the flow of your program inside that `main.py` file.

Lets see, lets create a new file in our directory called `myModule.py`:
```python
def greeting(name):
    print("hello" + name)
```
now we need to connect this module to our `main.py` file. And we can do this with the `import` statement. As it is in its name you simply import the code on a module:
```python
import myModule

myModule.greeintg("john")   # prints "hello, john"
```
You can rename your modules with `as` statement:
```python
import myModule as m

m.greeting(...)
```
By the way you will learn more about the startadt libraries down below but I wanted you to know that you import them this way too such as lets import the `random` standart library in our code:
```python
import random

# ... you can use random modules code here
```
And for heads up importing all of the code inside a module is a terrible idea. Usually lines of code ina mid sized application is between 10k to 100k lines of code. It is just inefficent to import all of them in your `main.py` you can just import the parts that you need and disregard the rest with `from` statement:
```python
from myModule import greeting

myModule.greeting("john")
```
If there were any other functions in `myModule` it coouldn't be used because in the above code they are not imported so basically they don't exist for `main.py`. There are much more you need to learn about import and modulairty in python. For example you need to learn about absolute and relative paths to learn how to access modules in different palces of your directory. You need to learn how to avoid circular imports .. etc. but all of the advanced stuff will be covered later on on my advanced python feynman note file. This just teaches you the basics and the logic behind it.

# Errors and Exceptions

So far we have learned most of the logic we needed to learn in python and programming. Now we need to learn a tirck and it is: "handling errors". What I mean by that is weather you are a star-unicorn programmer or a simple noob, you will ALWAYS run into errors. No code out there is error-free. So in order to survive int his distopyian world we need to have the correct control mechanims in place so that the program knows exactly what to do once the error is encountered. The logic is mostly same as control flows `if` blocks. But instead it is just designed for errors rather than implementing logic to check weather if it is true or false.

We have three new keywords to learn:
  - `try` -- block lets you test a block of code for errors
  - `except` -- block lets you handle the error
  - `finally` -- block lets you execute code, regardless of the result of the try-and-except blocks.
  
Lets see a basic example for starters:
```python
try:
  print(x)
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
```
The code above will execute the `except` block because the first code has an error in it (var x is not defined). So the thing you have to understand is that any single error made in the try block makes that block go to waste. So while using this error handling do not just put every bit of your code into these try ... except ... blocks. Only put code that you want to handle if it has errors in it. 

Because even though you might have an error in your code, maybe it is not that important and does not stops the core of your application from running. But if everyting was inside a giant try and except blocks the core of your program would not run becasue of a single small error in the try block. Remember to place these code blocks carefully and smartly.

There are many type of errors that you can raise with except. And we will learn them more in the future ...

# Files

...

# Additions

This section doesn't really have a name it is called `additions` because I am going to add new things to the note file in here. 

- `pass` -- the "pass" statement is a null statement. It doesn't really do anything. The only difrerence between a comment and a pass is that pass is interpreted by the interpreter while the comments are ignored. So most people use the pass statement as a placeholder value in functions, classes .. etc. so that poeple can comeback to it:
```python
function some_func_name():
    pass  # havent implemented anythign gonna get back to it later on
```
or 
```python
for val in sequence:
    pass
```

# Little tour of Standart Libraries

By now you have heard me blabber about this `standart library` in many parts of this note file. And it is farily easy to understand. Standart library is just a collection of `functions` that are created and maintained by the python's software foundation. Yes there are many more libraries (in millions) out there for you to use however the standart library comes pre-installed when you install python. They are not like 3rd party libraries where you need to install them from an outer source.

Now that we learned the library is just a collection of `functions` to be included in your own program. Lets define what are the standart libraries are:
- Serialization (`json` library) 
- File Wildcards (`glob` library)
- String Pattern Matching (`re` library)
- Mathematics (`math`, `random`, `statistics` libraries)
- Dates and Times (`datetime` library)
- Data Compression (`zlib` library)

Lets take a small look at each of these standart libraries. It is not logical to note all of their functionalities here because some of them are huge and they have their own documentation in place. 

- `json` -- you can use this library to serilize the json objects into python dictionaries, lists, tuples .. etc. If you are wondering what the hell is a json object do not worry it is beyond the scope of this note file. You will learn them once we get to API's in the backend section of this feynman-techniuqed-notebook.

- `glob` -- The glob module provides a function for making file lists from directory wildcard searches. Again if these words such as directory wildcard searching does not mean shit to you at the moment. Do not worry we will learn more about them in the operating system/shell subjects.

- `re` -- The re module provides regular expression tools for advanced string processing. For complex matching and manipulation, regular expressions offer various functions to use. Well yes regular expression is a vague term too but it is mostly about string manipulation, matching ... etc. it is not a hard thing to understand. When you want to build advanced programs you will almost always or most of the time run into string problems. And this module should always be in your toolbelt once you run into those type of problems.

- `math`, `random`, `statistics` -- well as it is in its name, these modules are extremly useful for various mathematical functions. They provide extremly well writen code for any math related concepts such as formulas, equations, high level mathematics such as calculus .. etc. People who code game engines, physics engines use these module extensively.

- `datetime` -- Suprisingly date time is an extremly tricky concept. Even the smartest people in the world gets confused by it. Because to be honest in order to get the fucking time you have to know about solar system and when and where our earth is currenlty located on the solar system ... etc. If you are a normal person such as me you will not have a built-in-house space observatory sysstem. So use this module to manipulate dates and time in your code.

- `zlib` -- Common data archiving and compression formats are directly supported by modules including: zlib,
gzip, bz2, lzma, zipfile and tarfile. To be fair this isn't a vagaue concept to be understood yes most of the commands will be unfamiliar but zlib basically lets you compress and archive your data such as winrar if you remember it.
