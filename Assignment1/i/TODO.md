1 .What is the difference between the two sum function given below?

// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}

// the first function returns he sum as a result that can be further used in the code. the second function logs the sum in the console but des not return it. this function is more used for debugging purposes.

//

2.If we store the returned value of both functions above in variable first and second what will be the value of first and second.

// for the first sum function 
let first = sum(3,4)
The returned value of sum(3, 4) is the result of the addition operation, which is 7.

for the second sum function
let second = sum(3,4)
the second sum function does not return any value exiplicitly; it only log the sum in the console. therefore the value of the second sum will be undefined.
//

3.What will be the output when you call above sum function (first) with three parameter like sum(12, 24, 35). Explain why?

// when we call the sum function with three parameter, only the first two parameters will be used in the addition operation.the third parameter will get ignored beacuse he function definition only specifies two parameters `a` and `b`. and the output will be `36`.
//

4.Can you store the first sum function in a variable named add. If yes why? If no why?



5.Declare a function named sayHello the accepts a parameter name and returns the name like Hello Arya.

function sayHello(name) {
  return `Hello Arya`;
}

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
 let message = 'Hello, ' + userName;
 return message;
}

showMessage();
-output will be Hello, John as function return variables from ourside also.

What will be the output for Output1 Output2 and Output3 in the code below.
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1  

showMessage(); // Output 2

alert(userName); // Output 3
output 1 will alert john while it is undefined. -output 2 will be Hello, John.
output 1 will alert john while it is undefined.
What is a Anonymous Function give example of three functions.
-Anonymous Function is a function that does not have any name associated with it. Normally we use the function keyword before the function name to define a function in JavaScript, however, in anonymous functions in JavaScript, we use only the function keyword without the function name. example - 1

var anon = function() {
  alert('I am anonymous');
}
anon();
example-2 arrow function

var anon = x => x + 1
example-3 arrow with brackets

var anon = x => {return x + 1}

9. Can function declaration be a Anonymous Function? Explain.

 - yes function declaration be a anonymous function by arrow operator as well as i had given example above.

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
function get() {
  return `return a value`
}
function calc() {
  return `calculate something`;
}
function create() {
  return `create something`
}
function check() {
  return `check something and return a boolean, etc`
}
function show() {
  return `show something`
}