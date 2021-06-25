---
title: "Printing"
post_type: "lecture"
---

# Printing

```python
print("Hello World")
```

In Python, printing is how we display information to the _console_.

```
Hello World
```

---

# Printing (Variations)

```python
# Anything in quotation marks can be printed
# without any problems
print("Hello World!")

# Numbers can be printed too
print(12345)

# You can print multiple things at the same
# time separated by a space by using commas
print("I am", 10, "years old")
```

- Numbers don't need `"`

```
Hello World!
12345
I am 10 years old
```

---

# Print without newlines

```python
print(1, end='')
print("hello", end='')
print("world")
```

By default, each `print` statement adds a _newline_ at the end. We can override this behavior by supplying an alternative ending.

```
1helloworld
```

---

# Comments

```python
# this dont do nothing
print("hello world")  # neither does this
```

- Anything after a `#` is a comment.
- Comments do not affect your code in any way
- Good for jotting down notes in your code
- You can select multiple lines and toggle comments by using `ctrl` + `/` (or `cmd` + `/`)

```
Hello World
```

---

# Data Types

```python
print(123)
print(3.14)
print(True)
print("I am a String!")
```

There are 4 primitive data types in Python

- int - whole numbers
- float - decimals
- bool - True/False
- str - anything in quotation marks

---

# Why is type important?

1. Different types have different operations
2. Different types don't get along (very well)

---

# Types and operations

```python
print( 3 / 4 + 4 * 3 )
print( "Hello" + "World" )
```

- Arithmetic operations for numbers
- Strings can be added (called concatenation) but cannot, for example, be divided

```
12.75
HelloWorld
```

---

# Different Types do not get along

```python
print(1 + "Hi")
print(True + 3.14)
print(True + "")
print("HEllo" / 4)
```

Every statement here is erroneous. **In general**, operators evaluate only the like types.

---

# Exception

```python
print("Hello" * 3)
print(1 + 3.14)
```

There are some exceptions to the rule, of course.

```
HelloHelloHello
4.140000000000001
```

---

# Type Casting

```python
print(float(3))
print(str(123))
print(int(3.5))
```

Type casting allows us to convert one data type to another.

- Floats are always _rounded down_.

```
3.0
123
3
```

---

# Type casting (cont)

```python
print(1 + int("3"))
print(3.14 + float("3.14"))
print("hi" + str(1))
```

```
4
6.28
hi1
```

---

```python
print(1 + int("1"))
print(str(1) + "1")
```

A subtle difference can make a huge impact on the outcome. (Lesson: Don't be sloppy)

```
2
11
```

---

# Invalid conversion

```python
x = int("hi")
```

Invalid typecasting will fail
