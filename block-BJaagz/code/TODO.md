1. Implement `forEach` array method using Array.reduce

- `forEach` accepts two parameter array and callback
- It does not return anything
- It should work exactly like array `forEach` method

```js
function forEach(num,cb) {
   num.reduce((acc,cv,i,arr)=> {
       // forEach doesn't return anything 
       cb(cv,i,arr);
      //  console.log(acc); - output will be sam
   });
}

forEach(['Sam', 'Jon', 'Arya'], (name, i, arr) =>
  console.log(name + name, i, arr)
);
```
// array.reduce rule if initial value is not passed then index 0 value will become initial value and passed to acc .

2. Implement `map` array method using Array.reduce

- `map` accepts two parameter array and callback
- It returns same size of array
- It should work exactly like array `map` method

```js
function map(array,cb) {
  // Your code goes here
  return array.reduce((acc,cv,i,arr)=>{
        acc.push(cb(cv,i,arr));
        return acc;
   },[]);
}

let output = map(['Sam', 'Jon', 'Arya'], (name) => name + name); // ['SamSam', 'JonJon', 'AryaArya']
console.log(output);
```

3. Implement `filter` array method using Array.reduce

- `filter` accepts two parameter array and callback
- It returns same size or smaller array
- It should work exactly like array `filter` method

```js
function filter(array,cb) {
  // Your code goes here
  return array.reduce((acc,cv,i,arr) => {
      if(cb(cv,i,arr)){
            acc.push(cv);       
      }
       return acc;
  },[])
}
filter(['Sam', 'Jon', 'Arya'], (name) =>
  name.startsWith('S')
); // ['Sam']
```
