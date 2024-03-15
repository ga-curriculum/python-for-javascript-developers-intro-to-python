# ![Intro to Python - Variables](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

## Python Variables

Variables in Python hold the data an app needs when it runs. 

### Declaring

Here is how we declare a variable in Python:

```python
my_number = 15
```

You cannot just declare a variable without assigning to it: 

```python
# illegal syntax...
my_variable
# returns: NameError: name 'my_variable' is not defined
```

### Naming Convention

Variables are case sensitive - variables named `my_number` and `My_Number` would be two different variables.

When you have a variable name with multiple words, the convention is to **snake_case** the identifier:

```python
# In Python we use snake_case...
my_number = 10
```

### Reassigning Variables

We can freely assign a new value to a variable after it has been declared: 

```python
my_number = 15
print(my_number)  
# prints 15
my_number = -4
print(my_number)
# prints -4
```

Reassignment replaces the current value, and the previous value becomes no longer available.