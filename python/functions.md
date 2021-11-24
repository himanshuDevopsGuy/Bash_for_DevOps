# Functions 


## Types of Functions in python
- userdefined Functions
- Builtin Functions

# Custom functions
## Definition

```
def function_name():
  add=1+2
  print(add)
```

## <ins> FUNCTIONS </ins>

- Python Functions is a block of related statements designed to perform a computational, logical, or evaluative task.
- The idea is to put some commonly or repeatedly done tasks together and make a function so that instead of writing the same code again and again for different inputs, we can do the function calls to reuse code contained in it over and over again. 
- Functions can be both built-in or user-defined. It helps the program to be concise, non-repetitive, and organized.
 

Syntax:
```python
def function_name(parameters):
    """docstring"""
    statement(s)
    return expression

function_name()
```

Example:

```python
def ot-python-scripters():
    print ('hello world')


ot-python-scripters()
```

output:

```
hello world
```

## <ins> FUNCTIONS [PARAMETER]</ins>

- Information can be passed into functions as arguments.
- Arguments are specified after the function name, inside the parentheses. You can add as many arguments as you want, just separate them with a comma.

From a function's perspective:

- A parameter is the variable listed inside the parentheses in the function definition.
- An argument is the value that is sent to the function when it is called.


Syntax:

```python
def ot-python-scripters(name):
    print (f'hello {name}')


ot-python-scripters("opstree")
```

Output:

```
hello opstree
```

Another example:

```python
def ot-python-scripters(first_name, second_name):
    print(f'{first_name} : {second_name}')

ot-python-scripters('Ops', 'tree')
ot-python-scripters('tech', 'primo')
```

Output:

```
Ops : tree
tech : primo
```


## <ins> FUNCTIONS [KEYWORD ARGUMENT] </ins>

- You can also send arguments with the key = value syntax.
- This way the order of the arguments does not matter.

Example:

```python
def ot-python-scripters(first_name, second_name):
    print(f'{first_name} : {second_name}')

ot-python-scripters(first_name='Ops', second_name='tree')
```

Output:

```
Ops : tree
```

## <ins> RETURN STATEMENT </ins>

- To let a function return a value, use the return statement.
- If we dont return any value, the answer will be always `None`.

Example:

```python
def ot-python-scripters(number):
    return number * number


result = ot-python-scripters(3)
print (result)
```

Output:

```
9
```

## <ins> GLOBAL VARIABLE </ins>

- Variables that are created outside of a function are known as global variables.
- Global variables can be used by everyone, both inside of functions and outside.

Example:

```python
x = "awesome"           ## Global variable
def myfunc():
  statement(s)          ## x value pick from global
myfunc()
```

- If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.


Example:

```python
x = "value1"        ## Global variable
def myfunc():
  x = "value2"      ## Function variable
  statement(s)
myfunc()
statement(s)
```

- Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.
- To create a global variable inside a function, you can use the global keyword.


```python
def myfunc():
  global var        ## local variable behave like global variable
  statement(s)
myfunc()
statement(s)
```

Function Description
abs() Returns the absolute value of a number
all() Returns True if all items in an iterable object are true
any() Returns True if any item in an iterable object is true
ascii() Returns a readable version of an object. Replaces none-ascii
characters with escape character
bin() Returns the binary version of a number
bool() Returns the boolean value of the specified object
bytearray() Returns an array of bytes
bytes() Returns a bytes object
callable() Returns True if the specified object is callable, otherwise False
chr() Returns a character from the specified Unicode code.
classmethod() Converts a method into a class method
compile() Returns the specified source as an object, ready to be executed
complex() Returns a complex number
delattr() Deletes the specified attribute (property or method) from the
specified object
dict() Returns a dictionary (Array)
dir() Returns a list of the specified object's properties and methods
divmod() Returns the quotient and the remainder when argument1 is divided by
argument2
enumerate() Takes a collection (e.g. a tuple) and returns it as an enumerate
object
eval() Evaluates and executes an expression
exec() Executes the specified code (or object)
filter() Use a filter function to exclude items in an iterable object
float() Returns a floating point number
format() Formats a specified value
frozenset() Returns a frozenset object
getattr() Returns the value of the specified attribute (property or method)
globals() Returns the current global symbol table as a dictionary
hasattr() Returns True if the specified object has the specified attribute
(property/method)
hash() Returns the hash value of a specified object
help() Executes the built-in help system
hex() Converts a number into a hexadecimal value
id() Returns the id of an object
input() Allowing user input
int() Returns an integer number
isinstance() Returns True if a specified object is an instance of a specified
object
issubclass() Returns True if a specified class is a subclass of a specified
object
iter() Returns an iterator object
len() Returns the length of an object
list() Returns a list
locals() Returns an updated dictionary of the current local symbol table
map() Returns the specified iterator with the specified function applied
to each item
max() Returns the largest item in an iterable
memoryview() Returns a memory view object
min() Returns the smallest item in an iterable
next() Returns the next item in an iterable
object() Returns a new object
oct() Converts a number into an octal
open() Opens a file and returns a file object
ord() Convert an integer representing the Unicode of the specified
character
pow() Returns the value of x to the power of y
print() Prints to the standard output device
property() Gets, sets, deletes a property
range() Returns a sequence of numbers, starting from 0 and increments by 1
(by default)
repr() Returns a readable version of an object
reversed() Returns a reversed iterator
round() Rounds a numbers
set() Returns a new set object
setattr() Sets an attribute (property/method) of an object
slice() Returns a slice object
sorted() Returns a sorted list
staticmethod() Converts a method into a static method
str() Returns a string object
sum() Sums the items of an iterator
super() Returns an object that represents the parent class
tuple() Returns a tuple
type() Returns the type of an object
vars() Returns the __dict__ property of an object
zip() Returns an iterator, from two or more iterators
