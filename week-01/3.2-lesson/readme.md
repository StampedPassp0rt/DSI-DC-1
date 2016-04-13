---
title: Anaconda, Jupyter Notebooks, CSV Library
duration: "1:5"
creator:
    name: Lucy Williams
    city: DC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Anaconda, Jupyter Notebooks, CSV Library
Week 1 | Lesson 3.2

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Demonstrate how to use the Jupyter notebook, code vs Markdown mode
- Show how to save and share the notebook via Jupyter
- Intro to csv library

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
- Install Anaconda
- Create an Anaconda environment with Jupyter Notebook installed


### LESSON GUIDE
| TIMING  | TYPE  | TOPIC  |
|:-:|---|---|
| 5 min  | [Introduction](#introduction)   |  Anaconda, iPython notebook, Jupyter, Code vs. Markdown, and csv library |
| 10 min  | [Demo / Guided Practice ](#demo)  | Anaconda  |
| 10 min  | [Demo / Guided Practice ](#demo)  | iPython notebook  |
| 10 min  | [Demo / Guided Practice ](#demo)  | Jupyter  |
| 10 min  | [Demo / Guided Practice ](#demo)  | Code vs. Markdown  |
| 10 min  | [Demo / Guided Practice ](#demo)  | csv library  |
| 30 min  | [Independent Practice](#ind-practice)  |  |
| 5 min  | [Conclusion](#conclusion)  |   |



<a name="Anaconda, Jupyter notebook, Code vs. Markdown, and csv library"></a>
## Introduction: (5 mins)

Anaconda is a completely free Python distribution. It includes more than 400 
of the most popular Python packages for science, math, engineering, and data analysis.
[Anaconda](https://www.continuum.io/downloads)

The Jupyter Notebook is a web application that allows you to create and share 
documents that contain live code, equations, visualizations and explanatory text. 
Uses include: data cleaning and transformation, numerical simulation, 
statistical modeling, machine learning and much more.
[Jupyter](http://jupyter.org/)

Lastly, we will take a peek at the csv library. 

<a name="Anaconda"></a>
## Demo / Codealong: Anaconda (10 mins)

For those of you who haven't installed Anaconda yet. Please go to the 
[Anaconda website](https://www.continuum.io/downloads) and follow the install 
instructions for your OS. Any questions, please ask the instructor, TA, or a 
fellow student. 

Before we take a look at Jupyter notebook, lets take a look at some of the other reference materials that come with Anaconda. 

<a name="Jupyter Notebook: Code vs. Markdown"></a>
## Demo / Codealong: Code vs. Markdown (10 mins)

Let's play around with Jupyter Notebook first to get a feel for it. Let's create a new notebook by clicking on the "New" dropdown and selecting under "Notebooks", "Python 2". Let's change the title right away to
something like "Practice", so we can easily ID it later. 

The notebook starts off in the "Code" mode, which means that the cell is ready to accept
any code we write. Let's toggle it to "Markdown" mode. [This is a great Markdown tutorial.](http://www.markdowntutorial.com/lesson/3/) 

Practice writing a cell of code and
then a cell of Markdown and run it. 

Next, click through the dropdown menus: File, Edit, View, Insert, Cell, Kernel, and Help, 
just to get a look at what's available. Don't worry, you'll become more familiar with 
these through usage. 


<a name="csv module"></a>
## Demo / Codealong: csv module (10 mins)

Let's take a look at the Python csv module. The csv module’s reader and 
writer objects read and write sequences. We'll be using a small Sales data set
to practice. Let's read a csv file first. 
[demo code](https://github.com/lucywi/dsi-course-materials/blob/master/curriculum/04-lessons/week-01/3.2-lesson/code/Demo%20Code%20-%20Week%201%20Lesson%203.2%20-%20Anaconda%2C%20Jupyter%20Notebooks%2C%20CSV%20Library.ipynb)

In Jupyter notebook type: 
```python
import csv
import urllib2

url = 'https://raw.githubusercontent.com/lucywi/dsi-course-materials/master/curriculum/04-lessons/week-01/3.2-lesson/assets/datasets/sales.csv?token=AGCAl_fr7Cv1EJ84zQ2Uy1igaitiqMhAks5XFuDpwA%3D%3D'
response = urllib2.urlopen(url)

# Opening a file with the mode 'U' or 'rU' will open a file for reading in universal newline mode.
with open('sales.csv', 'U') as f:
    reader = csv.reader(f)
    for row in reader:
        print row
f.close()
```

The output will be the contents of sales.csv file. Now, let's write to a csv file. 

In Jupyter notebook type: 
```python
b = open('writeTest.csv', 'w')
a = csv.writer(b)
data = [['Me', 'You'], \
        ['Hello', 'Goodbye'], \
        ['Monday', 'Friday']]
a.writerows(data)
b.close()
```

Now, let's see the file again, with the data you just added: 
```python
with open('writeTest.csv', 'U') as f:
    reader = csv.reader(f)
    for row in reader:
        print row
f.close()
```


<a name="ind-practice"></a>
## Independent Practice: Topic (30 minutes)
- Practice creating an Jupyter Notebook that uses both code and MarkDown cells. 
- Practice reading and writing csv files. 


<a name="conclusion"></a>
## Conclusion (5 mins)
Today we were introduced to Anaconda, Jupyter notebook, and how to read and write csv files. 
Nice. Next we'll be introduced to NumPy. Sounds like fun!
