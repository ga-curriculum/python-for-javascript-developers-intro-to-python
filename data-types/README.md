# ![Intro to Python - Data Types](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to check for and convert between Python Data Types.

## Data Types in Python

Python is very object-oriented.

Every piece of data in Python is an object that’s an instance of a *class*.

### Checking the Data Type (class) of an Object

We use the type() function to obtain the class used to instantiate the data:

```shell
>>> type(42)
<class 'int'>
>>> type('hello')
<class 'str'>
>>> type(True)
<class 'bool'>
```

Python’s data types are similar to those available in JavaScript, there’s just more of them.

### Integer Numbers (<class 'int'>)

Unlike in JavaScript, Python distinguishes between integers (whole numbers) and floats (numbers with decimals).

When we don’t follow a number literal with a decimal point, an integer is assumed:

```shell
>>> some_int = 25
>>> type(some_int)
<class 'int'>
```

We can force numbers to act as integers in some mathematical operations, as we will see. Doing this can force an integer result which is usually the same as calling `Math.floor()` in JavaScript.

### Floating-point Numbers (<class 'float'>)

Numbers with a decimal point are stored in variables as floating-point numbers, usually just called a `float`.

```shell
>>> pi = 3.14159
>>> type(pi)
<class 'float'>
>>> some_float = 25.
>>> type(some_float)
<class 'float'>
```

### Complex Numbers (`<class 'complex'>`)

Python even has a data type for complex numbers, i.e., numbers with an “imaginary” component usually obtained by taking the square root of a negative number.

The imaginary portion is represented by the letter ‘j’:

```shell
>>> my_complex = 3+4j
>>> type(my_complex)
<class 'complex'>
```

### Booleans (`<class 'bool'>`)

Named after George Boole, these are the logical data types often used in conditional expressions.

Just like in JS, we have `true` and `false` but spelled slightly differently:

```shell
>>> my_bool = True
>>> my_other_bool = False
>>> type(my_bool)
<class 'bool'>
```

Notice how they start with capital letters! You must start them with capital letters in Python or they will not reflect the boolean values.

### Nothingness (`<class 'NoneType'>`)

Similar to how JS has the `null` value to represent nothingness, Python has a similar value:

```python
my_nothing = None
```

The value `None` in Python, with a capital N, provides the same meaning as `null` does in JavaScript.

## Converting Between Data Types

One thing we kind of took for granted in JavaScript was that it usually performed automatic data type conversion for us - a process known as implicit type coercion.

```javascript
let numTacos = 25;
let msg = 'There are ' + numTacos + ' tacos';
msg => There are 25 tacos
```

However, in Python we cannot do this - there is no type coercion. With few exceptions, variables must be the same type to perform an operation on them.

Luckily, doing math operations between integers and floats is allowed, but not much else.

When the time comes to convert one data type into another, Python provides us with several global functions or predefined classes to do so:

```python
str(item)        # Converts the item to a string
int(item, base)  # Converts the item to an integer with the provided base
float(item)      # Converts the item to a floating-point number
hex(int)         # Converts an integer to a hexadecimal STRING
oct(int)         # Converts an integer to an octal STRING
tuple(item)      # Converts item to a tuple
list(item)       # Converts item to a list
dict(item)       # Converts item to a dictionary
```

