---
title: "Pure Functions"
date: "2021-03-03"
post_type: "lecture"
---

# Definition of Pure Function

- Given the same input, will always return the same output
- Produces no side effects

# Examples of pure functions

```js
function add(a, b) {
  return a + b;
}
```

```js
function reverse(arr) {
  let rev = [];
  for (let i = 0; i < arr.length; i++) {
    rev[i] = arr[arr.length - 1 - i];
  }
  return rev;
}
```

# Examples of non-pure functions

```js
// uses external variable
function increment() {
  x++;
}
```

```js
// does not return the same value for same input
function rand(x) {
  return Math.random() + x;
}
```

```js
// changes the input
function reverse(arr) {
  let l = 0,
    r = arr.length - 1;
  while (l < r) {
    let t = arr[l];
    arr[l] = arr[r];
    arr[r] = t;
    l++;
    r--;
  }
}
```

# Why is pure-function important?

- Pure functions are used heavily in Functional Programming. 
- Libraries such as **ReactJS** and Redux use them
- Ease of testing and refactoring
