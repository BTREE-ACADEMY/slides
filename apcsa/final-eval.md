---
title: "Final Evaluation"
date: "2021-03-19"
post_type: "lecture"
---

# Arrays and Loops

Q. Determine the resulting value of `x`

```java
int arr[] = { 1, 2, 3, 4, 5 };
int x = 0;
for(int i=0; i<arr.length; i++) {
  if (arr[i] % 3 != 0)
    x += arr[i];
}
```

---

Q. Determine the output

```java
for (int i = 1; i <= 3; i++) {
    for (int j = 0; j < i; j++) {
        System.out.println(i);
    }
}
```

---

Q. Code the following pattern

```none
*-*-*
*-*-
*-*
*-
*
```

# Errors

Q. When does the following code NOT work?

```java
public int findMin(int[] arr) {
  int min = 0;

  for(int v : arr) {
    if (v < min) {
      min = v;
    }
  }

  return min;
}
```

Q. find all errors and classify the types. (compile-time vs run-time)

```java
int a = 3.14;
double b = 3;

int c = (int) (a * b);

if ( a / b > 0 && b != 0) {
  System.out.println("infinite");
} else if (a != 0 && b / a > 0) {
  System.out.println("finite");
}
```

# ArrayList

Q. What are the remaining values of `list`?

```java
ArrayList<Integer> list = new ArrayList<>();
list.add(1);
list.add(0);
list.add(0);
list.add(0);
list.add(1);

for(int i=0; i<list.size(); i++) {
  if (list.get(i) == 0)
    list.remove();
}
```

# OOP

Q. Find all that's wrong

```java
public class A {
  static int a;
  int b;

  public A(int b) {
    this.b = b;
  }

  public int fn() {
    return a + b;
  }

  public int fn(int v) {
    return a + b + v;
  }

  public static int getA() {
    return a;
  }
  public static int getB() {
    return b;
  }
}
```

# OOP - inheritance

Q. Consider the following two classes,

```java
class A {
    public void fn() {
        System.out.println("1");
    }
}

class B extends A {
    public void fn() {
        super.fn();
        System.out.println("2");
    }
}
```

What would be the results of the following code segments?

```java
A obj = new A();
obj.fn();
```

```java
B obj2 = new A();
obj2.fn();
```

```java
A obj3 = new B();
obj3.fn();
```

```java
B obj4 = new B();
obj4.fn();
```

Q. Consider these two classes

```java
class A {
    int v = 10;

    public void fn() {
        System.out.println(v);
    }
}

class B extends A {
    int v = 20;

    public void fn() {
        super.fn();
        System.out.println(v);
    }
}
```

What would be the result of the following code snippet

```java
B obj4 = new B();
obj4.fn();
```

Q. Consider

```java
class A {
    int v = 10;

    public void fn() {
        System.out.println(v);
    }

    public void ahh() {
        fn();
    }

}

class B extends A {
    int v = 20;

    public void fn() {
        super.fn();
        System.out.println(v);
    }

    public void ahh() {
        super.ahh();
    }
}
```

What would be the result of the following code snippet

```java
B obj4 = new B();
obj4.fn();
```

# Misc.

Q. Determine the output

```java
int[] a = { 1, 2, 3 };
int[] b = a;
b[0]++;

System.out.println(a[0] + b[0]);
```
