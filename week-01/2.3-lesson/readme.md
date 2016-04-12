# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Intro to Python 4
Week 1 | Lesson 2.3

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Iterate using for loops
- Iterate using while loops

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- If you have time, watch a video on for and while loops so that you're familiar
  with the topic.

<a name="for and while loops"></a>
## Introduction: Loops (10 mins)
<details>
<summary>
What's a loop?
</summary>
```bash
A device that tells Python to do the same thing over and over again.
```
</details>

### For Loops

The for loop is used to iterate over the elements of a sequence.

You can use any object (such as strings, arrays, lists, tuples, dict and so on) in a for loop in Python.

The while loop tells the computer to do something as long as a condition is met.

###While Loops

A while loop consists of a block of code and a condition. The condition is evaluated, and if the condition is true, the code within the block is executed. This repeats until the condition becomes false.

[for and while loops](http://www.pythonforbeginners.com/control-flow-2/python-for-and-while-loops)
[for and while loops](http://www.cyberciti.biz/faq/python-for-loop-examples-statements/)


<a name="for loops"></a>
## Demo / Codealong: for loops (25 mins)

In script.py:
```bash
# basic for loop example
for count in [1, 2, 3]:
    print(count)
    print('Yes' * count)
```

This is a for loop. It has the heading starting with for, followed by a
variable name (count in this case), the word in, some sequence, and a final colon.
As with function definitions and other heading lines, the colon at the end of
the line indicates that a consistently indented block of statements follows
to complete the for loop.

Let's try a simple repeat for loop. When you just want to repeat the exact same
thing a specific number of times. In that case only the length of the sequence,
not the individual elements are important.

In script.py type:
```bash
# simple repeat loop
for i in range(10):
    print('Hello')
```

Let's try a for loop through words.
In script.py type:
```bash
# using a for loop to go through the letters in a word
word = 'computer'
for letter in word:
    print letter
```

Let's try using a for loop to print out a list.
In script.py type:
```bash
shuttles = ['columbia', 'endeavour', 'challenger', 'discovery', 'atlantis', 'enterprise', 'pathfinder' ]

for s in shuttles:
    print s
```

[for loops](http://www.cyberciti.biz/faq/python-for-loop-examples-statements/)
[for loops](http://www.pythonforbeginners.com/control-flow-2/python-for-and-while-loops)
[for loops](http://anh.cs.luc.edu/python/hands-on/3.1/handsonHtml/loops.html)

Group practice
Work with a partner for 10 minutes and write your own code for a for loop. You may be asked to come up and show your code.

<a name="while loops"></a>
## Demo / Codealong: while loops (25 mins)

Let's create a simple counter using a while loop.
In script.py type:
```bash
# create a counter using a while loop
count = 0
while count < 5:
    print count
    count = count + 1  
```

Let's try another.
In script.py type:
```bash
# another counter using a while loop
a = 0		
while a < 10:
   a = a + 1
   print a
```

And maybe one more...
In script.py type:
```bash
while True:
    reply = raw_input('Enter text, [type "stop" to quit]: ')
    print reply.lower()
    if reply == 'stop':
        break
```

This while loop will stop when the user types "stop".

Remember, a while loop runs until the expression is False. The problem is,
sometimes they don't stop. To avoid this, here are some rules to follow:

1. Make sure that you use while-loops sparingly. Usually a for-loop is better.
2. Review your while statements and make sure that the boolean test will
   become False at some point.
3. When in doubt, print out your test variable at the top and bottom of the
   while-loop to see what it's doing.

[while loops](http://learnpythonthehardway.org/book/ex33.html)

Group Practice
Work with a partner for 10 minutes and write your own code for a for loop. You may be asked to come up and show your code.


<a name="conclusion"></a>
## Conclusion (5 mins)
- When is a for loop useful?
- When is a while loop useful?
- What are the differences between for and while loops?
- What is a problem that while loops run into?
- What are some things you can do so you don't run into this problem with while loops?
