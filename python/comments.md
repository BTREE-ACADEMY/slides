---
title: "Logical Operators"
date: "2021-03-13"
marp: true
post_type: "lecture"
---

Let's first see if the following sentence makes sense:

> In order to be classified as a teenager, you must be older then 12 or younger than 20.

---

> In order to be classified as a teenager, you must be older then 12 **or** younger than 20.

This sentence is _incorrect_ because we used _or_ instead of _and_. Using _or_ allows all ages to qualify (union) whereas _and_ only takes the intersection.

In this chapter we will take a closer look at these two logical operators `and` and `or`.

---

# `And` and `Or`

When we have to combine multiple booleans into a single one, we often use these two logical operators. Even though we use them somewhat interchangeably in real life, they are two very different things. Take a look at these two examples:

> You must pass vision **and** hearing tests to get your driver's license

> You must have a credit **or** debit card.

---

# Truth table

To describe exactly how `and` and `or` works, we often turn to what's known as a truth table. 

|  P  |  Q  | P and Q | P or Q |
| :-: | :-: | :-----: | :----: |
|  T  |  T  |    T    |   T    |
|  T  |  F  |    F    |   T    |
|  F  |  T  |    F    |   T    |
|  F  |  F  |    F    |   F    |

In summary, `and` requires both operands to be true whereas `or` only requires one of the two conditions to be true.

---

# Exercise

```py
x = 10
```

Throughout this exercise, the value of x will be 10 and won't change. Determine what each of the following lines will print:


```py
print ( 1 < x )
print ( x <= 20 )

print ( 1 < x < 20 ) 

print ( x == 10 or 20 ) 
print ( x == 10 or x == 20 ) 

print ( 1 / 0 > 0 and True ) 
print ( True or 1 / 0 > 0 ) 
print ( False and 1 / 0 > 0 ) 
print ( False or 1 / 0 > 0 ) 

print ( x > 1 or x < 10 )
print ( x < 1 and x > 20 )
```

