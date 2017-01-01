# Python Quick Start

Python is a widely used programming language (source code is now available under the GNU General Public License – GPL) started by [Guido van Rossum](http://en.wikipedia.org/wiki/Guido_van_Rossum) that supports multiple programming paradigms.

Although it is an interpreted language rather than compiled language, hence might take up more CPU time (important detail in our Computer Architecture department), Python has a gentle learning curve, Python is readable, writeable, and endlessly powerful. Its simplicity lets you become productive quickly. 

This hand-on will show some basic characteristics of Python to help to enter those **students of my course who have no prior knowledge of python**. At the end of the page you will find very useful links to advance on your own and some tips that could help you.  

## How to install Python?

We can install Python 2 or Python 3. This is one of the debated topics in Python. There is no right/wrong choice here, specially if you are a beginner. Python 2 has an awesome community support, plethora of third-party libraries. On the other hand Python 3 is cleaner and faster. For the purpouse of this hands-on it is not important, the student should focus on learning Python as a language. For advice on choosing between Python 2 and Python 3 see [Python 2 or 3](https://wiki.python.org/moin/Python2orPython3).

Before you start, you will need Python on your computer, but you may not need to download it. Nowadays many Linux and UNIX distributions include a recent Python. Even some Windows computers now come with Python already installed. First of all check that you don’t already have Python installed by entering python in a command line. If you see a response from a Python interpreter it will include a version number in its initial display. If you use are in a environment you will see:

``` 
torres@vm:~$ python
Python 2.7.10 (default, Sep 23 2015, 04:34:14) 
[GCC 4.2.1 Compatible Apple LLVM 7.0.0 (clang-700.0.72)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```
For Warming up you can run your first Python program. You can use Python as a simple calculator to start with:
``` 
>>> 15+10
25
>>> 
```
Congratulations, good job!

If you need to install Python, you can download the most recent stable version of Python 2 or Python 3 from [general download page](https://www.python.org/downloads/).

## Python basics
###Line indentation

Python has no mandatory statement termination characters and blocks are specified by indentation (there are no braces to indicate blocks of code for class and function definitions or flow control). Statements that expect an indentation level end in a colon (:). The number of spaces in the indentation is variable, but all statements within the block must be indented the same amount. Python will advise you if there is a unclear line indentation with the following warning:

``` 

IndentationError: unexpected indent

```
Comments start with the pound (#) sign and are single-line, multi-line strings are used for multi-line comments.

###Variables and operators

Python is implicitly typed language (i.e. you don’t have to declare variables), case sensitive (i.e. Barcelona and BARCELONA are two different variables) and object-oriented (i.e. everything is an object). Help in Python is always available right in the interpreter. Type *help()* for interactive help, or *help(object)* for help about object. If you want to know how an object works, all you have to do is call *help(\<object\>)* Also useful are *dir()*, which shows you all the object’s methods:


```

>>> help (int)

Help on int object:
class int(object)
| int(x=0) -> int or long
| int(x, base=10) -> int or long
| 
…

| Methods defined here:
| 
| __abs__(…)
| x.__abs__() <==> abs(x)
…

(type q to exit)

```
The addition, subtraction, multiplication, and division operations work just like expected. In addition we can use the modulus operator (\%). All the modulus operator does is to divide the left side by the right side and get the remainder. The floor division operator (\/\/) just divides the number and rounds down. The double * is just an easy way to provide exponents to Python.

Values are assigned with the sign “=”, in fact, objects are bound to names (the equality testing is done using two equal signs “==”). It is possible use the += and -= operators on many datatypes, strings included. You can also use multiple variables and swaps variables in one line. It doesn’t violate variable typing because values aren’t actually being assigned, but new objects are bound to the old names.

``` 
>>> IntegerVar = 10
>>> IntegerVar += 10
>>> print IntegerVar
20
>>> StringVar = “Welcome”
>>> StringVar += ” to Barcelona”
>>> print StringVar
Welcome to Barcelona
>>> IntegerVar, StringVar = StringVar, IntegerVar
>>> print IntegerVar
Welcome to Barcelona
>>> print StringVar
20
>>> help (StringVar)
Help on int object:

class int(object)
| int(x=0) -> int or long
| int(x, base=10) -> int or long
| 
…

```
###Data types

## Development environment

Alternately, you can download and install a package, which comes with pre-installed libraries. I would recommend for beginners downloading [Anaconda](https://www.continuum.io/downloads) available for Windows, OS X or Linux, 32- or 64-bit.
Another option could be [Enthought Canopy Express](https://store.enthought.com/downloads/#default). I personally prefer iPython Notebooks from Anaconda because it provides a lot of good features for documenting while writing the code itself and you can choose to run the code in blocks rather than the line by line execution in the terminal environment. We will use iPython environment for this complete hands-on tutorial.

You can start iPython notebook by writing “ipython notebook” on your terminal:
``` 
torres@vm:~$ ipython notebook

```
You can create a new iPython notebook by simply clicking on the **new** button  in the top. The interface shows **In\[\*\]**  for inputs and **Out\[\*\]** for output. You can execute a code by pressing *“Shift + Enter”* or *“ALT + Enter”*, if you want to insert an additional row after.




