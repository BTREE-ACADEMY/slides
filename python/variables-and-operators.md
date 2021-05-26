---
title: "Hello World"
date: "2021-03-03"
post_type: "lecture2"
---

# Hello World 🌎

```python
print("Hello World")
```

Print hello world

```none
Hello World
```


---

## `print()` options

```python
print("print text");
print(10);
```

To output anything to the console we use the `print()` function. Note that numbers do not need quotation marks.

```
print text
10
```

---

```python
print("1 + 1 is", 1 + 1)
```

We can use comma `,` to print multiple objects onto a single line

```
1 + 1 is 2
```

---

```python
print("1", end="\n")  # default behavior
print("2", end="")
print("3")
```

We can override the default _ending_ behavior.

```
1
2 3
```

---

# Comments

```python
# prints hello world
print("Hello World!")
```

Comments will not affect the code. Used to leave notes to yourself or others

You can easily comment or uncomment multiple lines of code by `ctrl` + `/`

---

# Variables

```py
x = 10
print(x)

x = 20
print(x)
```

You can store data in a variable. Data stored in a variable will be preserved until changed later.

```
10
20
```

---

## Types

```python
a = 1
b = 3.14
c = True
d = "Hello"
```

Here are the 4 basics (called _primitive_) data types:

- Integer (whole numbers)
- Float
- Boolean (true or false)
- String (text)

---

```python
x = 5
print(type(x))
```

You can obtain the type of a variable using the `type()` function, but probably won't ...

```html
<class 'int'>
```

---

```python
print(1 + 1)
print("1" + "1")
print(1 + "1")
```

More importantly, know that _different types cannot interact with each other_. Each type also behaves differently with operators. Remember this. This thing is important.

```
2
11
ERROR
```

---

## Casting

```py
x = int("1")
y = float("2.0")
z = int("hello")   # obviously won't work 🙄
```

you can (try to) change a type of variable to another type

---

# Don't be sloppy! 🤪

```python
x = "1"
y = 20
z = 10

print( The sum of x+y+z = (x + y + z)  )

x = 1
y = 2
print("sum of x+y = ", "x" + "y")
```

It's unfair to expect you (or anyone) to memorize everything right away. Feel free to make mistakes so you can learn from them. However, when you do make a mistake, please stop and think about why the code does not work so it will not happen again. Here, I showcase a few buggy codes. Try to predict and fix the errors.

