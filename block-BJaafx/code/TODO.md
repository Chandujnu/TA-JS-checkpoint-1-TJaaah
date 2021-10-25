1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
function averageOfNumnber() {
  let sum = 0;
   
for(i = 1; i <= 10; i++) {
  let input = +prompt(`Enter numbers`);
  sum += input;
 }
 alert (`The average is ${sum / 10}`);
}
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
// Output will throw an error as println is not defined.
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum (max = 10) {
  let sum = 0;
  for (i = 1; i <= max; i++) {
    if(i % 2 == 0) {
      sum += i;
    }
  }
  return `The sum of all even numbers is ${sum}`;
} 
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum(max = 10) {
  let sum = 0;
  for(i = 1; i <= max; i++) {
    if (i % 2 !=0) {
      sum +=i;
    }
  }
  return `The sum of all odd mumbres is ${sum}`;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

```js
function getProductOfDigits(num) {
  let i = num, m = 1, digit;
  while (i) {
    digit = i % 10;
    if (digit) m *= digit;
    i = Math.floor(i / 10);
  }
  return m;
} 
```
- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // `Bigger than 5`, Because condition is that if num is greater than 5, it will return `Bigger than 5`
check(1); // `Smaller than 5`, Because condition is that if num is smaller than 5, it will return `Smaller than 5`
check(5); // 5, As number itself is 5 and there is no condition it will return 5.
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // Here output will be `You are arya`, as in the condition if argument is `Arya`, output will be `You are arya`
getOutput('John'); // Here output will be `You are john`, as in the condition if argument is `John`, output will be `You are john`
getOutput(); // Here output will be `Who are you`, as in the condition if argument is other than `Arya` and `John`, output will be `Who are you`
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // Here output will be `You are arya`, and again it will return the value `Who are you` as in the condition if argument is `Arya`, because console just print the output.
getOutput('John'); // Here output will be `You are john`, and again it will return the value `Who are you` as in the condition if argument is `John`, because console just print the output.
getOutput(); // Here output will be `Who are you`, as in the condition if argument is other than `Arya` and `John`, output will be `Who are you`
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
Ans:- 
```js
// No, a function  can't have multiple return statement,because it will only return either true or false statement, but only one.
function equalNumber (a, b) {
  if(a == b) {
    return `${a} and ${b} are equal`;
  } else {
    return `${a} and ${b} are not equal`;
  }
}

// Here also we will get only one return statement. 
```


10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

Ans:- 
```js
// Difference between `for` loop and `while` loop is that in `for` loop first statement is executed and then we increment or decrement the value, but in `while` loop we can increment or decrement the value either before or after the statement, in `for` loop if the condition is not satisfied it execute infinite times, but in `while` loop when condition is not satisfied it shows error, because `while` loop first check the codition. And we can use `for` loop when we already know the number of iteration and when we don't know the number of iteration we use `while` loop.
 
 for (i = 0; i < 10; i = i+1) {
   if (i % 2 == 0) {
     console.log(i);
   }
 }

 // while loop 

while (i < 10) {
  if (i % 2 == 0) {
    console.log(i);
  }
  i = i+1;
}