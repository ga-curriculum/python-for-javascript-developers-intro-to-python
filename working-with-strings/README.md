# ![Intro to Python - Working with Strings](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to write strings, perform string interpolation, and use string methods to work with string types in Python.

## Working with Strings

Python also has strings for holding text, just like JavaScript:

```python
my_string = "A double quoted string"
your_string = 'A single quoted string'
```

You can also do some multi-line strings by using a triple quote (single or double):

```python
multiline_string = '''This is my string that
                        goes on multiple lines
                          for whatever reason'''
```

### Concatenating Strings

One or more strings can be combined into a single string in the same way we do it in JS, by using the `+` operator:

```python
little_string = "bad"
medium_string = "super"
long_string = medium_string + little_string
print(long_string)
# prints "superbad"
```

### String Interpolation using f-Strings

One fancy thing that Python has had much longer than JavaScript is a nice syntax for string interpolation (evaluating Python expressions and embedding the result within strings).

While we can always use the concatenation operators above, these get ugly when too many of them appear in a string. Instead, we can use syntax similar to what was introduced in ES6 with string template literals. You just need to remember to add an `f` before the string:

```python
state = "Hawaii"
year = 1959
message = f"{state} was the last state to join the U.S. in {year}."
```

When the `f` is placed directly before the opening quote (single, or double) of the string, it makes a formatted string or, **f-String**, for short.

Once we do this, we can put expressions into curly braces to “inject” the result of the expressions into the string.

f-Strings are awesome, but they’ve only been available since version 3.6.

Prior to f-Strings, there were a couple of other options, one being the string `format` method:

```python
template = "My name is {} and I like {}"
print( template.format("Ben", "tacos") )
# prints 'My name is Ben and I like tacos'
```

## Useful String Methods

Just like JS, Python has a number of string methods that we can use for string manipulation.

Some are familiar, like `split()` but others have different names:

```python
"ace of spades".split(" ")
# => ['ace', 'of', 'spades']

# However, this won't work
"abcd".split("")
# Instead, use the list() function like this:
list("abcd")
# => ['a', 'b', 'c', 'd']

"qqxzzz".index("x")    # Warning: Raises error if substring not found
# => 2

"boo".upper()
# => "BOO"

"WHY???".lower()
# => "why???"

"Then I went to the store I like".replace("I", "you")
# => 'Then you went to the store you like'
```

Want to know if a string contains a substring? You don’t even need a function for that. You can use the most excellent `in` operator to quickly find out if one string appears in another.

```python
"eggs" in "green eggs and ham"
# => True
```

Use the built-in global `len()` function on a string to find its length.

```python
len("Tacos")
# => 5
```

