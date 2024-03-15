# ![Intro to Python - Built in Functions](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will introduced to built in Python functions. 

Notice above that we did not call `len()` as a method on the string - we didn’t do this: `"Tacos".len()`.

`len()` is just one of several [**built-in functions**](https://docs.python.org/3/library/functions.html) that exists in Python.

`len()`, for example, is a function that returns the length (the number of items) of an object. The argument may be any sequence or collection (more on these tomorrow).

Why does `len()` work on strings? Because in Python, a string is a sequence of characters.

Because a string is a sequence, as we can in JS, we can use square brackets to access the characters in the string (but not assign to them, also like JS):

```python
course = 'SEI'
print( course[0] )
# => Prints 'S'

# We can use negative indices!
last_letter = course[-1]
print( last_letter )
# => Prints 'I'
```
