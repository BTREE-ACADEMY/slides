---
title: "Functions"
date: "2021-03-03"
post_type: "lecture"
---

_Functions_ are the first-class citizens in JavaScript. 🙄

# pre-requisite - primitive vs reference type

What is the value of `x`?

```js
let x = 10;
let y = x;
y++;
```

What is the value of `b[0]`?

```js
let a = [1, 2, 3];
let b = a;
a[0]++;
```

# define a function

```js
function add(a, b) {
  return a + b;
}
```

This is a special syntax that basically does the following (+hoistering):

```js
let add = function (a, b) {
  return a + b;
};
```

Just like any _reference type_ variables -- try naming a few -- function is just an _anonymous_ object that can be passed around.

For example, we can create an alias of `add()` simply by creating another reference.

```js
let sum = add;
sum(1, 2);
```

We can even add it to an array

```js
let ar = [add];
ar[0](1, 2);
```

We can pass it as a function paramter

```js
let add = function (a, b) {
  return a + b;
};

function fn(f) {
  console.log(f(1, 2));
}

fn(add);
```

We can return it as a return value

```js
let add = function (a, b) {
  return a + b;
};

function fn() {
  return add;
}

console.log(fn()(1, 2));
```

We can define an anonymous function anywhere

```js
function fn() {
  return function (a, b) {
    return a + b;
  };
}

console.log(fn()(1, 2));
```

We can also...

Alright, let's stop. 🛑

Take this as the _flexibility_, not a _difficulty_.

# Arrow Function

Since functions are used everywhere, JavaScript also provides a way to shorten the functions into what we call an **_arrow_function_**

```js
const add = function (a, b) {
  return a + b;
};
```

The equivalent arrow-function is (replace `function` with `=>`):

```js
const add = (a, b) => {
  return a + b;
};
```

If an arrow-function only has a single statement, just as is the case for `if` and `for`, we can omit the `{}` -- and the `return` statement.

```js
const add = (a, b) => a + b;
```

# pure functions

We define a _pure function_ by the following properties:

1. Identical return values for identical arguments - no randomness, no external effects
1. No side effects - no mutation of global(static) variables, input objects

example of a pure function

```js
function add(a, b) {
  return a + b;
}
```

example of a non-pure function
```js
function removeZero(ar) {
  for(let i=0; )
}
```

# exercise

Create the following _pure_ functions. Write as few lines as possible (after the auto-format):

```js
console.log(add(1, 2));
console.log(max(1, 2));
console.log(maxAr([1, 5, 4]));
console.log(rand(1, 3));
console.log(reverse([1, 2, 3]));
```
