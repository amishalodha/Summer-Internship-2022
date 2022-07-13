# Javascript quiz (Basic Level 4)

Q1 What are anonymous functions in JavaScript?

* An anonymous function is a function without a name.
* When we create an anonymous function, it is declared without any identifier. It is the difference between a normal function and an anonymous function.

``` javascript
let x = function () {  
    console.log('It is an anonymous function');  
};  
x();  
```
Q2 Explain strict comparison and Abstract comparison in javascript?

* Abstract equality will attempt to resolve the data types via type coercion before making a comparison. 
* Strict equality will return false if the types are different.
*  The difference between both the operators is that “==” is used to compare values whereas, “ === “ is used to compare both values and types.

 ```javascript
     var x = 2;
     var y = "2";
     (x == y)  // Returns true since the value of both x and y is the same
     (x === y) // Returns false since the typeof x is "number" and typeof y is "string"
```

Q 3 Difference b/w arrow functions and regular functions?

* Arrow function is one of the features introduced in the ES6 version of JavaScript. It allows you to create functions in a cleaner way compared to regular functions. 
```javascript
   let greet = () => console.log('Hello');
greet(); // Hello
```
* Regular functions created using function declarations or expressions are constructible and callable.Since regular functions are constructible, they can be called using the new keyword.
```javascript
    let square = function(x){

  return (x*x);

};

console.log(square(5));
```

Q 4  What is Hoisting in JavaScript?
* In JavaScript, Hoisting is a kind of default behavior in which all the declarations either variable declaration or function declaration are moved at the top of the scope just before executing the program's code.

Q 5 JavaScript is a garbage collected programming language, explain how?
* The main concept garbage collection relies on is the concept of references and reachability. It distinguishes between values that are reachable and values that are not. Values that are reachable are local variables and parameters in a current function. If there are nested functions in the chain, reachable values are also parameters and variables of these nested functions.

Q 6 Explain Shallow copy vs Deep copy in Javascript?
* A deep copy means that all of the values of the new variable are copied and disconnected from the original variable.
* A shallow copy means that certain (sub-)values are still connected to the original variable.

Q7 What is Object.freeze?
* Object.freeze() which is used to freeze an object. Freezing an object does not allow new properties to be added to an object and prevents from removing or altering the existing properties.

# PROGRAMS

Q 1 Write a function that generates a random number between two ranges, -100 to 0 and
800 - 900.

 ```javascript
     function randomNumber(min, max){

    return Math.random(Math.random()*(max-min+1) + min)
   }

    const Num1=randomNumber(-100, 0);

    const Num1=randomNumber(800, 900);

   console.log(Num1);

    console.log(Num2);
```


