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

# Functions

# Classes

# Input/Output

# Modules

# Errors and Exceptions

# Files

# Additions

# Little tour of Standart Libraries

By now you have heard me blabber about this `standart library` in many parts of this note file. And it is farily easy to understand. Standart library is just a collection of `functions` that are created and maintained by the python's software foundation. Yes there are many more libraries (in millions) out there for you to use however the standart library comes pre-installed when you install python. They are not like 3rd party libraries where you need to install them from an outer source.

Now that we learned the library is just a collection of `functions` to be included in your own program. Lets define what are the standart libraries are:
- Serialization (`json` library) 
- File Wildcards (`glob` library)
- String Pattern Matching (`re` library)
- Mathematics (`math`, `random`, `statistics` libraries)
- Dates and Times (`datetime` library)
- Data Compression (`zlib` library)
