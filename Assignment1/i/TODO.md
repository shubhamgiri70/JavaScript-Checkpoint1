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

// yes, we can store the first `sum` function in a variable named `add`. In JavaScript, functions are the first class citizens, so they can be treated as any other value in javascript, And we can assign them to the variables just like we would with strings,numbers or objects.
//

5.Declare a function named sayHello the accepts a parameter name and returns the name like Hello Arya.

function sayHello(name){
return `Hello Arya`
}

6. What will be the output of the function below and why?

````js
let userName = 'John';

function showMessage() {
 let message = 'Hello, ' + userName;
 return message;
}

showMessage();
// the output of the following will be `Hello, John`. because we already have a global variable named userName with the value `John`. and inside the function there is a local variable named `message` with the string `Hello, ` concatenated with the value of the global variable `userName`.
//

What will be the output for Output1 Output2 and Output3 in the code below.
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName);
// Output 1 will display an alert with the message 'John'.
//
showMessage();
// This statement calls the showMessage function. Inside the showMessage function, a message is constructed by concatenating the string 'Hello, ' with the value of the userName variable ('John'). So, output 2 will be Hello, John.
//

alert(userName);
// Output 3 will display an alert with the message 'John'.
//

What is a Anonymous Function give example of three functions.

// An Anonymous function is a function that does not have a name assign to it.

here is an example of three functions

Anonymous function //
let add = function(a, b) {
    return a + b;
}

arrow function with braces //
let add = (a, b) => {
   return a + b;
}

arrow function without braces //
let add = (a, b) => a + b;


9. Can function declaration be a Anonymous Function? Explain.

 - No, a function declaration cannot be an Anonymous function. a function declaration in JavaScript is a statement that defines a named function. In contrast, An Anonymous function is a function without name. it is define as a functin expression or an arrow funtion.

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

let name = 'Shubham';
function get(){
   return name + " " + 'Giri'
}

get()

function calc(totalstudents, presentstudents){
    return totalstudents - presentstudents;
}

calc();

function create(name, age){
    return my name is ${name} and i'm ${age} year old. 
}

create()

function check(age) {
    if (age > 18) {
        return "You can drive.";
    } else {
        return "You can't drive.";
    }
}

check()
````
