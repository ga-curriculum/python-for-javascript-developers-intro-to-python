# ![Intro to Python - Performing Operations](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

## Math Operations

Python has the normal math operators that you are used to from JavaScript:

- Addition `(+)`
- Subtraction `(-)`
- Multiplication `(*)`
- Division `(/)`
- Modulo (remainder) `(%)`
- Exponentiation `(**)`

All work as you would expect. However, there few other things worth mentioning: 

### Integer Division

It was mentioned earlier that you could force operands to act like integers to get an integer result. This is specifically enabled for division:

```shell
>>> quotient = 5 // 2
>>> quotient
2
# 2 is printed, because the decimal ".5" is truncated
```

### Shortcut Assignment Operators

As we saw in JS, the operation of reassigning to a variable the result of adding, etc. to that variable is so common, there are a number of shortcut operators in the language that make it cleaner to write.

Python has the very same operators: 

```python
# This line of code...
num = num + 1
# ...can be written with this shortcut operator:
num += 1

# It also works for any of the other math operations:
num = num / 5
# Rewrite like this:
num /= 5

# And this...
num = num * 3
# Can be written as this...
num *= 3
# And so on with the other operators.
```

> IMPORTANT: A couple of our favorites in JS, the Increment (++) and Decrement (--) operators, do not exist in Python. Use += 1 and -= 1 instead.


