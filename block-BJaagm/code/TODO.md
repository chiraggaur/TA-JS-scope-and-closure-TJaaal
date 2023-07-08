1. What does thread of execution means in JavaScript?
'''
thread of execution means line by line execution of code in js.
It will create gec and fec on the basis of line by line execution of code.
'''

2. Where the JavaScript code gets executed?
'''
js code executed in gec (global execution context).
'''
3. What does context means in Global Execution Context?
'''
GEC(global execution context) is created every time js code executed and it is created only ones.

'''

4. When do you create a global execution context.
'''
GEC is created in the very beigining of the execution of code and created only ones.
'''
5. Execution context consists of what all things?
'''
It is created of two spaces one for memory and other is for execution or computation happens.
'''

6. What are the different types of execution context?
'''
Gec and Fec(Function execution context).
'''

7. When global and function execution context gets created?

8. Function execution gets created during function execution or while declaring a function.


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)