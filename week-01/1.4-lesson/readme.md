# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Intro to Python 2
Week 1 | Lesson 1.4

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Create lists and operate on them
- Create dictionaries and operate on them

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- Define/describe/explain a list and a dictionary

<a name="introduction"></a>
## Introduction: Lists and Dictionaries (10 mins)

In our last lesson, we went over the six Python data types.

<details>
<summary>
What were they?
</summary>
```bash
- Integers
- Floats
- Strings
- Tuples
- Lists
- Dictionaries
```
</details>

Lists and dictionaries are the most fundamental data structures in Python. In this lesson, we'll be learning to create and perform operations on them.

Turn and Talk: Work in pairs and white table the definitions of list and dictionary.

<details>
<summary>
Lists
</summary>
```bash
- A collection of values
- Can be changed; not fixed
- Each value has a number associated with it, starting at 0
- Denoted by square brackets
```
</details>

<details>
<summary>
Dictionaries
</summary>
```bash
- A collection of key and value pairs
- Keys are unique, values are not
- Values can be of any data type, but keys must be immutable types (integer, string, tuple)
- No specific order of key, value pairs
```
</details>

[Lists and Dictionaries](http://sthurlow.com/python/lesson06/)


<a name="demo"></a>
## Guided Practice: Lists (30 mins)

Lists are similar to tuples.

<details>
<summary>
Why would we use a list over a tuple?
</summary>
```bash
- Lists are modifiable, tuples are fixed.
- Most of the time we use lists, not tuples, because we want to easily change the values of things if we need to.
```
</details>

Say you have five friends named Skeeter, Patty, Roger, Bebe and Porkchop. Let's create a list.

How do we create a list?

<details>
<summary>
In the Python shell type:
</summary>
```bash
friends = ['Skeeter', 'Patty', 'Roger', 'Bebe', 'Porkchop']
```
</details>

then type:
```bash
friends
```

Let's print the 3rd friend in your list.

<details>
<summary>
In the Python shell type:
</summary>
```bash
print friends[2]
```
</details>

<details>
<summary>
and it returns:
</summary>
```bash
Roger
```
</details>

Let's add to the list.

In the Python shell type:
```bash
friends.append('Doug')
```

then type:
```bash
friends
```

<details>
<summary>
and it returns:
</summary>
```bash
['Skeeter', 'Patty', 'Roger', 'Bebe', 'Porkchop', 'Doug']
```
</details>

append() is what we call a method for Python. Let's play around with a couple more.

Let's remove your 4th friend using del.

<details>
<summary>
In the Python shell type:
</summary>
```bash
del friends[3]
```
</details>

then type:
```bash
friends
```

<details>
<summary>
and it returns:
</summary>
```bash
['Skeeter', 'Patty', 'Roger', 'Porkchop', 'Doug']
```
</details>

Now let's see what the pop() method does.

In the Python shell type:
```bash
friends.pop()
```
What happens when you type:
```bash
friends
```
<details>
<summary>
it returns:
</summary>
```bash
['Skeeter', 'Patty', 'Roger', 'Porkchop']
```
</details>

[Lists](http://sthurlow.com/python/lesson06/)


<a name="ind-practice"></a>
## Group Practice: Topic (10 minutes)
Create your own list
Return only one element in the list
Add/delete something to the list


<a name="demo"></a>
## Demo: Dictionaries (30 mins)

Now you have a list of your friends, but let's say you want to store their favorite color to retrieve at another time.

You can't do this with a list. Here's where dictionaries come into play.



We know that dictionaries have keys and values.
In other words, your friends' names would be the keys and their favorite colors
would be the values.

When you initially create a dictionary, it is very much like making a tuple or list.
Tuples have ( and ) things, lists have [ and ] things. Guess what! Dictionaries
have { and } things - curly braces.

In the Python shell type:
```bash
# Make the phone book:
colors = {'Skeeter':green, 'Patty':blue, 'Roger':red, 'Porkchop':pink}
```

then type:
```bash
colors
```

and it returns:
```bash
{'Skeeter': green,
 'Patty': blue,
 'Roger': red,
 'Porkchop': pink}
```

Let's add a new friend to colors.
In the Python shell type:
```bash
colors['Doug'] = yellow
```

then type:
```bash
colors
```

and it returns:
```bash
{'Skeeter': green,
 'Doug': yellow,
 'Patty': blue,
 'Roger': red,
 'Porkchop': pink}
```

Let's delete a friend from colors.
In the Python shell type:
```bash
del colors['Roger']
```

then type:
```bash
colors
```

and it returns:
```bash
{'Doug': 'yellow',
 'Skeeter': 'green',
 'Patty': 'blue',
 'Porkchop': 'pink'}
```

Let's create a new dictionary with nothing in it to start with:
In the Python shell type:
```bash
ages = {}
```

Now, let's add some names and ages to the dictionary.
```bash
ages['Doug'] = 28
ages['Skeeter'] = 29
ages['Patty'] = 30
ages['Porkchop'] = 27
```

[Dictionaries](http://sthurlow.com/python/lesson06/)

<a name="ind-practice"></a>
## Group Practice: Topic (10 minutes)
Create your own dictionary
Return only one element in the dictionary
Add/delete something to the dictionary

<a name="conclusion"></a>
## Conclusion (10 mins)
- Partner up and explain what a list and a dictionary are to your partners
- What are the differences between a list and a dictionary?
- What are the two things you need for a dictionary?
