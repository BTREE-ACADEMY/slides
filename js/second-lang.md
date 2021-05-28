---
title: "JavaScript Syntax"
date: "2021-03-03"
post_type: "lecture"
---

# JavaScript for JAVA/Python programmers

JavaScript has a similar syntax as Java. Heck, it copied its name and also copied its syntax. JavaScript is now the [most popular language](https://insights.dice.com/2020/12/03/10-most-popular-programming-languages-on-github/) according to github.

# Editor

JavaScript runs natively on all modern browsers. (Try running JavaScript from the development panel). In this chapter, we will be using https://replit.com for convenience.

# Hello World

```js
console.log("Hello", "World");
```

# variables

```js
const x = 10;
let y = 20;
var z = 30;
```

`const` is self-explanatory. `var` is deprecated.

# types

- `Number`, `String`, `Array`... (no `char`)
- Types are not fixed

```js
let x = "hello";
x = "hi";
x = 10;
```

but obviously, don't do that...

# Operators

```js
+, -, *, /, %
+=, -=, *=, /=, %=
&&, ||, !
===, !==, >, <, >=, <=
```

Most notable of the above is the triple-equal sign `===`. JavaScript's `==` performs an auto-conversion. Meaning, that the following code returns true. This leniency is now considered 👿, so the community deprecated `==` and replaced it by `===`.

```js
1 == "1"; // true
1 === "1"; // false
```

**TL;DR**
Do not use `==`. Always use `===`

# `undefined`

Anything that's not defined is undefined.

```js
let x;
console.log(x); // prints "undefined"
```

To check if something is undefined

```js
if (x === undefined)
if (!x)
if (typeof x === 'undefined')
```

There is also a `null` value which is used similarly. The difference is that `null` does not natively occur. For the most part, use `undefined`.

# Shorthand `if` statements

These are used **very often**

```js
let x;
console.log(x || "N/A");
console.log(x && "x exists");
console.log(x ? "NOPE" : "YAY");

x = 10;
console.log(x || "N/A");
console.log(x && "x exists");
console.log(x ? "NOPE" : "YAY");
```

# functions

```js
function add(a, b) {
  return a + b;
}
```

Functions do not care about input or output types (Is this a good thing?)
More on _functions_ later...

# while

```js
let x = 0;

while (x < 10) {
  console.log(x);
  x++;
}
```

# for

```js
for (let x = 0; x < 10; x++) {
  console.log(x);
}
```

# arrays

```js
let ar = [1, 2, 3, 4, 5];
```

## traversal

```js
for (let i = 0; i < ar.length; i++) {
  console.log(ar[i]);
}

for (let key of ar) {
  console.log(key);
}
```

more on _arrays_ later...

# objects

aka `dictionary`, `hashmap`

```js
let ob = {
  A: 12,
  B: 20,
  C: 30
}

if ("C" in ob)
  console.log(ob.C)
```

## traversal

```js
for (let key in ob)
  console.log(ob[key])
```