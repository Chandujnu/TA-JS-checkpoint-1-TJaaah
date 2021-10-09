1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
// The difference between the first sum and second sum is that, the first one is returning the value but second one is consoling or printing the value.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
// Output will be 36 (12+34), because third parameter is not defined hence it will be left and only calculate first and second parameter.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
//Yes we can, because it is just function name.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function sayHello(name) {
  return `Hello ${name}`;
}
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage(); // `Hello, John`
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // `John`

showMessage(); // `Hello, John`

alert(userName); // `John`
```

8. What is a Anonymous Function give example of three functions.

When we define a function in a variable and remove the name of function, because it becomes of no use as function get stored in the variable, Thus it becomes anonymous function.
```js
// function declaration
function add(a, b) {
  return a + b;
}

// function expression
const addTwoNumbers = function add(a, b) {
  return a + b;
}

// function anonymous
const addTwoNumbers = function(a, b) {
  return a+ b;
}
// Arrow function
const addTwoNumbers = (a, b) => {
  return a + b;
}
    OR
const addTwoNumbers = (a, b) => a + b;

```

9. Can function declaration be a Anonymous Function? Explain
// Yes function declaration can be anonymous function by doing like this:-
```js

function add (a, b) {
  return a + b;
}
// This is a function declaration, and we can make it anonymous function
const add = function(a, b) {
  return a + b;
}

```

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
<!-- ```js -->
//
1. function add(a, b)
2. function substract(a,b)
3. function mult(a, b)
4. function div(a, b)
5. function sayHello(name)