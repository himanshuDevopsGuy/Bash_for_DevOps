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
def rawat():
    print ('hello world')


rawat()
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
def rawat(name):
    print (f'hello {name}')


rawat("rawat")
```

Output:

```
hello rawat
```

Another example:

```python
def rawat(first_name, second_name):
    print(f'{first_name} : {second_name}')

rawat('bhupi', 'rawat')
rawat('bhupi', 'singh')
```

Output:

```
bhupi : rawat
bhupi : singh
```


## <ins> FUNCTIONS [KEYWORD ARGUMENT] </ins>

- You can also send arguments with the key = value syntax.
- This way the order of the arguments does not matter.

Example:

```python
def rawat(first_name, second_name):
    print(f'{first_name} : {second_name}')

rawat(first_name='bhupi', second_name='rawat')
```

Output:

```
bhupi : rawat
```

## <ins> RETURN STATEMENT </ins>

- To let a function return a value, use the return statement.
- If we dont return any value, the answer will be always `None`.

Example:

```python
def rawat(number):
    return number * number


result = rawat(3)
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
