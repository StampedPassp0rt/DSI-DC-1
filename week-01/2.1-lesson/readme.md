# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Intro to Python 3
Week 1 | Lesson 2.1

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Write pseudocode
- Undersand control flow and execute conditional statements
- Define and invoke functions

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- Have a cursory explanation/idea of if/else, if/elif/else, loops, and functions.

## Morning Exercise/Psuedocode

<details>
<summary>
Psuedocode
</summary>
```bash
An informal but explicit description of the steps we want our computer to follow. It's intended for human reading rather than machine reading. To ensure that the computer skips over the psuedocode when reading your script, mark it
as a comment. In Python, a comment is designated by the # sign.
```
</details>

Now pretend I'm a computer, help me make a peanut butter and jelly sandwich. White table the instructions for me.


## Control Flow: Topic (10 mins)

So far, we've used Python to give our computer a sequence of instructions to follow one after another. But it's often
the case that the flow of a program will need to be altered to accommodate a particular situation. Here's where the concept of control flow comes into play.

<details>
<summary>
Control flow
</summary>
```bash
Statements that enable a program to execute different sequences of instructions based on the case at hand. This essentially allows the program to "choose" an appropriate course of action.
```
</details>

[control flow](http://www.codeproject.com/Articles/663666/Python-Basics-Understanding-The-Flow-Control-State)


<a name="if, if/else"></a>
## Demo if, if/else (15 mins)
The general Python syntax for a simple if statement is:
```bash
        if condition :
            indentedStatementBlock

```

If the condition is true, then do the indented statements. If the condition
is not true, then skip the indented statements.

So far, we've been working in the Python shell. Now, let's make a Python script in our text editor. Create a new file in Atom and call it script.py. The 'py' file extension is how you let
your computer know that it's reading a Python script. You can run it in the terminal by typing python script.py

```bash
weight = float(input("How many pounds does your suitcase weigh? "))
if weight > 50:
        print("There is a $25 charge for luggage that heavy.")
print("Thank you for your business.")
```
FYI: Float and input are built-in Python functions. Here's a list of more: https://docs.python.org/2/library/functions.html#built-in-funcs

In script.py type:
```bash
43
```
<details>
<summary>
and it returns
</summary>
```bash
Thank you for your business.
```
</details>


Now type:
```bash
75
```
<details>
<summary>
and it returns
</summary>
```bash
There is a $25 charge for luggage that heavy.
Thank you for your business.
```
</details>


The general Python if-else syntax is

        if condition :
            indentedStatementBlockForTrueCondition
        else:
            indentedStatementBlockForFalseCondition

These statement blocks can have any number of statements, and can include
about any kind of statement. The else is executed ONLY after the computer has determined that the first condition
wasn't met.

In script.py type:
```bash
age = float(input('How old are you? '))
```

then type:
```bash
if age >= 21:
    print('Have a beer with me at the GA Happy Hour, my friend')
else:
    print('I think we have some juice for you')
print("You're never too young or too old to learn data science")
```

[control flow statements](http://anh.cs.luc.edu/python/hands-on/3.1/handsonHtml/ifstatements.html)


<a name="if/elif/else"></a>
## Demo: if/elif/else (15 mins)
The syntax for an if-elif-else statement is indicated in general below:

        if condition1 :
            indentedStatementBlockForTrueCondition1
        elif condition2 :
            indentedStatementBlockForFirstTrueCondition2
        elif condition3 :
            indentedStatementBlockForFirstTrueCondition3
        elif condition4 :
            indentedStatementBlockForFirstTrueCondition4
        else:
            indentedStatementBlockForEachConditionFalse

In script.py type:
```bash
x = int(raw_input("Please enter an integer: "))
```

Type in an integer.

then type:
```bash
if x < 0:
    print 'Negative'
elif x == 0:
    print 'Zero'
elif x == 1:
    print 'Single'
else:
    print 'More'
```
The if, each elif, and the final else line are all aligned. There can be any number
of elif lines, each followed by an indented block. With this construction exactly
one of the indented blocks is executed. It is the one corresponding to the first
True condition.

Note: Check out comparison operators here: http://www.tutorialspoint.com/python/python_basic_operators.htm

[control flow statements](http://anh.cs.luc.edu/python/hands-on/3.1/handsonHtml/ifstatements.html)

<a name="functions"></a>
## Demo: functions (15 mins)
<details>
<summary>
What's a function?
</summary>
```bash
Think of a function as a small program inside a program. The basic idea is that we write a sequence of statements and then give that sequence a name.
```
</details>

You can define functions to provide the required functionality. Here are simple rules to define a function in Python.

Function blocks begin with the keyword def followed by the function name and parentheses ( ( ) ).

Any input parameters or arguments should be placed within these parentheses. You can also define parameters inside these parentheses.

The first statement of a function can be an optional statement - the documentation string of the function or docstring.

The code block within every function starts with a colon (:) and is indented.

The statement return [expression] exits a function, optionally passing back an expression to the caller. A return statement with no arguments is the same as return None.


The syntax for a function is indicated in general below:
```bash
def functionname( parameters ):
   "function_docstring"
   function_suite
   return [expression]
```

Let's create a function called printme
In script.py type:
```bash
def printme( str ):
   "This prints a passed string into this function"
   print str
   return
```

But it's not enough to define a function. Now, we need to 'call' it, in order for the function to be invoked:
```bash
printme("hello, it's me")
```

and it returns:
```bash
hello, it's me
```

[defining a function](http://www.tutorialspoint.com/python/python_functions.htm)

<a name="ind-practice"></a>
## Pair Practice: Topic (10 minutes)
- What is the general syntax/format of:  
        -  if/else?
        -  if/elif/else?
        - function?
- Define, white table and explain each to a partner

<a name="conclusion"></a>
## Conclusion (5 mins)
Today we learned about if/else, if/elif/else and functions. Practice coding each until you
feel comfortable. If you understand basic control flow concepts, you're on your way to writing
fantastic executable programs!
