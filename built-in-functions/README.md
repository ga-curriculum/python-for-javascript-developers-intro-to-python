# ![Python for JavaScript Developers - Intro to Python - Built-in Functions](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be familiar with some of Python's built-in functions.

## Working with built-in functions

You might have noticed that when we used `len()` in the previous lesson, we did not call it as a method on the string. Put another way, we didn't write `"Tacos".len()`. Instead, we wrote `len("Tacos")`.

`len()` is one of Python's [built-in functions](https://docs.python.org/3/library/functions.html). The `len()` function accepts any sequence or collection as an argument. It returns that sequence or collection's length (the number of items in it).

Why does `len()` work on strings? Because in Python (like JavaScript), a string is a sequence of characters.

This is also why we were able to use another one of Python's  built-in functions: `list()`. We used it with the code `list("abcd")`!

## Strings as sequences

We can even use square brackets to access the individual characters as we could in JavaScript:

```python
greeting = "Hello"
print( greeting[0] )
# prints: 'H'

# Python lets us use negative indices!
last_letter = greeting[-1]
print( last_letter )
# prints: 'o'
```

Although we can access individual characters in a string, we cannot change them because strings are immutable, again, just like they are in JavaScript:

```python
greeting[0] = "Y"
# TypeError: 'str' object does not support item assignment
```
