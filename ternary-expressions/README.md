# ![Intro to Python - Ternary Expressions](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

### Ternary Expressions

In JS we used the ternary expression to concisely return one of two values depending upon a conditional expression, for example:

```javascript
// Using the ternary operator/expression
let beverage = age >= 21 ? 'Beer' : 'Milk';

// Without a ternary expression
let beverage;
if (age >= 21) {
  beverage = 'Beer';
} else {
  beverage = 'Milk';
}
```

Python, however, does not have a dedicated ternary operator. Instead, Python uses a modified syntax of `if`/`else` which results in a ternary expression instead of a control flow construct.

The Python ternary expression equivalent to the JS example above is:

```python
beverage = 'Beer' if age >= 21 else 'Milk'
```
