1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
```
let score = function (marks, total) {
  return (marks * 100) / total;
}

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
```
Function Declaration

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```
 Function Expression

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```
 Function Expression

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```
 Function Expression

```js
let percentage = (marks, total) => (marks * 100) / total;
```
 Function Expression

 '''
3. Why is a function definition an expression in JavaScript? Give one example of function expression.

'''
function defination is a expression in js because function is a object in js and object can be written as expression .

'''
4. Why is a function call an expression in JavaScript?

'''
function call is a expression in js because function is a object in js and object can be written as expression .

'''

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer - valid
five = add; // Answer - invalid
five = five(10, 11); // Answer - invalid
five = function () { 
  return 'Hello';
}; // Answer - invalid 
```

6. What is the difference between function definition and function call? Explain with an example.

'''
function defination is the series of steps to perform something , where as function call is execution  of the series of steps already defined.
'''


7. What is the similarities between function definition and function call?
'''
function defination and function call have same name of the function on which both works on.

'''

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid
```
'''
invalid because function is not call or executed. hello();

'''
9. What is higher order function explain with an example.
'''
when function is passed as a parameter or function return a function is called hof.
'''

10. Explain what is callback function. Why you can pass a function inside a function?
'''
when function is passed as an argument is called call back function.
'''
