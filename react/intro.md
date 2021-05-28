---
title: "Intro"
date: "2021-03-03"
post_type: "lecture"
---

# What is React?

A framework that allows you to build Facebook-quality apps (i.e. pretty much all apps) using JavaScript.

# What does "Using JavaScript" mean?

Normally, you would create an `.html` file for each page of your website. With React, you can create a single `.js` file to _generate_ all of your pages dynamically.

For example, to build the following buttons:

<button>😀</button><button>😁</button><button>😁</button><button>😄</button><button>😄</button><button>🤩</button><button>🙂</button><button>😚</button><button>😣</button><button>🤩</button><button>😘</button><button>😥</button><button>😯</button><button>😶</button><button>🙄</button>

manual html

```html
<button>😀</button>
<button>😁</button>
<button>😁</button>
<button>😄</button>
<button>😄</button>
<button>🤩</button>
<button>🙂</button>
<button>😚</button>
<button>😣</button>
<button>🤩</button>
<button>😘</button>
<button>😥</button>
<button>😯</button>
<button>😶</button>
<button>🙄</button>
```

react

```js
{
  "😀,😁,😁,😄,😄,🤩,🙂,😚,😣,🤩,😘,😥,😯,😶,🙄"
    .split(",")
    .map((v) => <button>{v}</button>);
}
```

Using JavaScript also comes with the added benefit of interactivity.

# Pros and Cons

**PROS**
It's really good. The development paradigm of React is so good that it has become (subjectively) the de-facto standard of a lot of development frameworks for web and to some extent, mobile and desktop apps as well.

**CONS**
Steep learning curve. You need to learn a lot about JavaScript. Good Luck 🍀!

# I already know HTML/CSS

Good. You can miss the first 1/2 of week 3. But all of the knowledge will still be re-used.

HTML Tags: `body`,`h1`,`div`,`span`,`input`,`form`,`img`,`li`,`a`

CSS Props: `font-size`,`font-weight`,`color`,`background`,`margin`,`padding`,`border`,`box-shadow`,`border-radius`

CSS Selectors: `class`,`child`,`descendent`,`:not()`,`-nth-child`

# I already know Flex-box (really well)

Good. You can miss the entire week 3. We will use flex-box throughout this class.

Flex properties: `display: flex`,`justify-content`,`align-items`,`align-content`,`flex-grow`,`flex-shrink`

# I already know jQuery

Great. They will help a lot. Keep in mind that you won't use any jQuery directly here, as React and jQuery do not share the same methodologies. 

# There will be a test!

On HTML,CSS,FLEXBOX

👉 Accuracy
👉 Speed
👉 Open Book

# Sign Up

https://codesandbox.io - React

https://replit.com - To Learn JavaScript

https://github.io

# Local Installation

1. node.js
2. git
3. vs code

Installation videos will be posted... soon...

# GOAL

1. Portfolio of in-class projects
2. Portfolio of homework projects
3. Personal Portfolio project
4. Win [congressional app challenge](https://www.congressionalappchallenge.us/)
5. Launch a startup
6. Become a millionaire
7. Have an app I can brag about

# Skills you WILL master

1. HTML/CSS
1. JavaScript
1. React

