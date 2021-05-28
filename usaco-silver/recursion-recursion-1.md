---
title: "Recursion 1"
date: "2021-03-03"
post_type: "lecture"
---

# Recursion

Definition: a function that calls itself.

```java
void fn() {
  System.out.println("hi");
  fn();
}
```

`fn()` will print "hi" forever -- hence not a very good example but it serves the purpose of showing us what a recursion is.

# Why is it important?

In short, *recursion can do everything that a loop can do*, **plus more**. However, it's a bit slower. Compare these two:

```java
for(int i = a; i < b; i++)
  System.out.println(i);
```

```java
int print(int a, int b) {
  if (a == b)
    return;
  System.out.println(a);
}
```

In general, we would prefer loops over recursion if possible. In this chapter, we will force ourselves to use recursion over for loops. In the next chapter, we will look at questions that can only be done using recursion.

# Trace

First step to learning recursion is tracing.