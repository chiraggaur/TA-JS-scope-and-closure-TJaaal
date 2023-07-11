Create the execution context diagram for the following code snippets:

```js
function outer() {
  let b = 10;
  function inner() {
    let a = 20;
    console.log(a + b);
  }
  return inner;
}
let getSum = outer(); //output  - innerfunction (){}
let num = getSum(); //output  -  log 20+10 = 30 , due to closure b = 10 ;
```
'''
created diagram in notebook
'''

2.

Create the execution context diagram for following code. Also write the output of the code below.

```js
function getCounter() {
  let count = 0;

  return () => {
    return count++;
  };
}

let counter = getCounter(); // counter will carry returning function along with count = 0 due to closure;

counter(); // output - 0
counter(); // output - 1
counter(); // output - 2
counter(); // output - 3 
```
'''
created diagram in notebook
'''
3. Create the execution context diagram

```js
function makeColorChanger(color) {
  return function () {
    document.body.style.backgroundColor = color;
  };
}

let blue = makeColorChanger('blue'); //it will carry function along with color = 'blue';
let tomato = makeColorChanger('tomato');//it will carry function along with color = 'tomato';

blue(); // output - bg color = blue
tomato();// output - bg color = tomato

// What will be the background color after the execution of last line
```
'''
created diagram in notebook
'''