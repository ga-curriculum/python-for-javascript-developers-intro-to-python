# ![Python for Javascript Developers - Intro to Python - Built in Functions](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will introduced to built in functions in Python.

In the previous lesson, we did not call `len()` as a method on the string: `"Tacos".len()`.

`len()` is just one of several [**built-in functions**](https://docs.python.org/3/library/functions.html) that exists in Python.

For example, `len()`, is a function that returns the length (the number of items) of an object. The argument may be any sequence or collection.

Why does `len()` work on strings? Because in Python, a string is a sequence of characters.

Because a string is a sequence, like in JavaScript, we can use square brackets to access the characters (but not assign to them, also like JavaScript):

```python
greeting = 'Hello'
print( greeting[0] )
# => Prints 'H'

# We can use negative indices!
last_letter = greeting[-1]
print( last_letter )
# => Prints 'o'
```
