Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // output
```
In the above code we are looking for 'username'. It is not a global variable as it is declared with (const)inside block scope and we can't access it from outside the block.

 The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```
In the above code we are looking for 'username'. It is not a global variable as it is declared with (const)inside block scope and we can't access it from outside the block.

 The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // output - Arya
```
In the above code we are looking for 'username'. It is not a global variable but as it is declared with (var) inside block scope and we can access it from outside the block.

 The above code will // output - Arya

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output // error it  is if scope 
```
In the above code we are looking for 'username'. It is a global variable with let  also it is declared inside block scope but as it is declared with (var) inside block scope but as per rule var only follow function thats why we can't redeclared it with same name.

 The above code will throw an error `Uncaught SyntaxError: Identifier 'username' has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output - John
```
In the above code username is declared with let but it is declared in global and block scope seprately which is allowed thats why we can acess the global scope only from outside the block and the output is John .



7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output - John  
```
In the above code we are looking for 'username'. It is a global variable also it is declared inside with let inside function scope which is not accesible from outside.

The above code will give output John 

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output - (0-9,First);  
}
console.log(i, 'Second'); // output - 10 ,'Second;
```
In the above code we are looking for 'i'. It is declared with var in for loop and var only follow block and function block;

It will give output first complete the for loop and then  at 10 it will exit loopn and console the value of i ie - 10 now;


9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
In  the above code i is dclared with let which follow block scope thats why ionly 0-9 , First will console and after the loop it will through error Reference Error i is not defined