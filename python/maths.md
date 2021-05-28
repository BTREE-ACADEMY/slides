---
title: "Maths! 🧮"
date: "2021-03-03"
post_type: "lecture"
---

`int` and `float` types can participate in mathematical operations. i.e. we can add, subtract, divide and multiply number types. Standard math rules apply:

- Associativity
- Precedence
- **One operation at a time**

---

# 🏹 One at a time RULE

When a statement contains multiple operators, Python takes them 1 at a time according to the rule of precendence. For example,
`x = 10 + 2 * 3` contains 3 operators (can you count them?). The first operator is a `*`. After evaluating the operator, the statement becomes `x = 10 + 6`.

What happened here is that `2 * 3` just _became_ `6`. We, as coders, say that _"2 times 3 **returns** 6"_. Remember the word "returns"

---

# Arithmetic Operators

- `+` Addition
- `-` Subtraction
- `*` Multiplication
- `/` Division
- `//` Integer division
- `%` Modulus (Remainder)

---

## Division

`/` operator performs the typical mathematical division. Nothing much to say here...

```python
1 / 3 = 0.333
2 / 3 = 0.666
3 / 3 = 1
4 / 3 = 1.333

100 / 3 = ?
101 / 3 = ?
```

Keep in mind that, in general, we try to stay away from using floats due to their precision issues.

---

## Division into quotient and remainder

14 / 4 gives us Q=3 and R=2. That is

```
14 = 3 * 4 + 2
```

We have `//` and `%` for quotient and remainder. As far as this course is concerned, these two operators are more important then `/`. -- again, to avoid floats.

```python
14 // 4 = 3
14 % 4 = 2
```

---

## Integer Division

This one should be very easy. It's practically taking the _ceiling_.

```python
1 // 3 = 0
2 // 3 = 0
3 // 3 = 1
4 // 3 = 1
5 // 3 = 1
6 // 3 = 2
7 // 3 = 2
```

---

## Modulo

This one might be new to you. However, you will be using modulus _a lot_ going forward so take time and master how mod(%) works.

```python
3 % 3 = 0
4 % 3 = 1
5 % 3 = 2
6 % 3 = 0
7 % 3 = 1
8 % 3 = 2
9 % 3 = 0
```

---

A couple of popular usages of modulo is (1) checking the oddity and (2) extracting the last digit

```py
7 % 2 = 1
10 % 2 = 0
122 % 2 = 0
43221 % 2 = 1

12345 % 10 = 5
```

---

## Exponentiation

```python
print(2 ** 3)     # prints "8"
```

---

## Exercise

Write the expected values

```python
print(2 + 3)
print(2 - 3)
print(2 * 3)
print(2 / 3)
print(2 // 3)
print(2 % 3)
print("1" + "1")
```

---

# Assignment Operators

When we create a variable we have been using the `=` operator to assign its value. In Python, this is called an assignment operator. We _assign_ the value on the right to the value on the left.

```python
x = 5
print(x)
x = 10
print(x)
x = 15
print(x)
```

---

Remember that the variable being updated is the one on the left. What would be the values of `x` and `y` after the following codes? Run your code to find out.

```python
x = 10
y = 20
x = y
print(x, y)
```

---

Now consider this example:

```python
x = 10
y = 20
x = y + 10
x + 10 = y
```

Line 3 changes `x` to 30, as `y + 10` evaluates to 30. However, line 4 does not work. The left hand side of the `=` should always be a variable, not an expression.

---

Note that without the `=`, variables do not change their values. Consider the following code.

```python
x = 10
print(x + 10)
print(x)
```

This code prints 20 and then 10, not 20. `print(x+10)` does not change the value of `x`.

---

# increment, decrement

Sometimes, you might want to change a variables value based on its previous value.

Let's suppose we have a variable `hp` representing a health point of a character in a game. With each hit, the character loses 1 HP.

```python
hp = 100
hp = hp - 1
hp = hp - 1
```

Or more simply,

```python
hp = 100
hp -= 1
hp -= 1
```

`hp -= 1` and `hp = hp - 1` are _identical_ in functionality, it is just quicker to write the former. We can do the same for all the other arithmetic operators. Try to guess the outcome (and run the code to find out!):

---

## Exericse

```python
x = 5

x += 5
print(x)

x -= 5
print(x)

x *= 5
print(x)

x //= 5
print(x)

x %= 5
print(x)
```

---

## Exercise

Determine the final value of `x`.

```python
x = 10
x = x + 5
x += 12
x -= 10
x *= 2
x //= 5
x -= x
print(x)
```

---

# Comparison Operators

```python
1 == 2
1 < 2
1 <= 2
1 > 2
1 >= 2
1 != 2
```

Comparison operators return a very special type of values called _booleans_. There are only 2 Boolean type values: `True` and `False`
