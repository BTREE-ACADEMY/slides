---
title: "React - Hello World"
date: "2021-03-03"
post_type: "lecture"
---

# hello world

```jsx
function App() {
  return (
    <div className="App">
      <h1>Hello World</h1>
    </div>
  );
}
```

The HTML-looking snippet is called **JSX**, and it is one of the core parts of React.

# State variable

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/00f8493f-c190-4162-bf25-92098b61e716/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/00f8493f-c190-4162-bf25-92098b61e716/Untitled.png)

```jsx
function App() {
  //let x = 3;
  let [x, setX] = useState(3);
  function increment() {
    setX(x + 1);
  }
  function reset() {
    setX(0);
  }
  function decrement() {
    setX(x - 1);
  }

  return (
    <div className="App">
      <h1>{x}</h1>
      <button onClick={increment}>+</button>
      <button onClick={reset}>reset</button>
      <button onClick={decrement}>-</button>
    </div>
  );
}
```

# Arrays

```jsx
function App() {
  let [ar, setAr] = useState([2, 2, 3, 10]);

  let btns = ar.map((v) => <button>{v}</button>);

  return (
    <div className="App">
      <div>{ar}</div>
      <div>{btns}</div>
    </div>
  );
}
```
