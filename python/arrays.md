---
title: "Arrays"
date: "2021-03-03"
post_type: "lecture"
---

# Init

```js
let ar = new Array(3); //  [undefined, undefined, undefined]
let ar = [1, 2, 3];
```

# print

```js
console.log(ar);
```

# traverse

```js
for (let i = 0; i < ar.length; ++i) {
  console.log(ar[i]);
}

for (let v of ar) {
  console.log(v);
}
```

# forEach

Another way to traverse an array is by using a forEach method

```js
ar.forEach(fn);
```

`fn` is called for every element of `ar` and is provided the (value, index) pair.

We usually define the function right inside the paranthesis

```js
ar.forEach((v, i) => console.log(v));
```

# map

`map` is a _pure function_ used extensively in React development. It returns a _new array_ containing a "mapped" value of each element from the original array.

```js
let ar2 = ar.map((v) => v * 2);
```

used to remove values from an array

```js
let a = [ 1, 2, 3, 4 ];
let b = a.filter(v => v == 2);
```

# Exercises

Create ***pure*** functions

Q. Calculate the maximum value of an array

```js
let max = 0;
ar.forEach((v) => max = max > v ? max : v)
```

Q. double every values in an array

```js
let b = a.map((v) => v * 2)
```

Q. replace even numbers with zeroes

```js
let b = a.map((v, i) => v % 2 === 0 ? a[i-1] : v)
```

Q. remove the first item

```js
let b = a.filter((v,i) => i > 0);
```