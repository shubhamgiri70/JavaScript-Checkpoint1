Using loops take 10 inputs from user and find the average of all the numbers.



What will be the output of the code below
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
// Uncaught ReferenceError: println is not defined //

Write a function named getEvenSum that accepts a parameter max. Return the sum of all even numbers. The value of max should default to 10.

// function getEvenSum(max = 10) {
    let result = 0;
    for (let i = 1; i <= max; i++) {
        if (i % 2 === 0) {
            result += i;
        } 
    }
    return result;
} 

getEvenSum() //

Write a function named getOddSum that accepts a parameter max. Return the sum of all odd numbers. The value of max should default to 10.

//function getOddSum(max = 10) {
    let result = 0;
    for (let i = 1; i <= max; i++) {
        if (i % 2 !== 0) {
            result += i;
        } 
    }
    return result;
}

getOddSum()//

Write a function named getProductOfDigits that accepts a parameter num. It returns the product of all the digits in the number.
If the input value is less than 0 return not a valid input
For example if the input is 123 output should be 6.

// 


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


check(10); // 'Bigger than 5'
check(1); // 'Smaller than 5'
check(5); // 5


What will be the output of the following code given below? Explain the reason?
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 
When calling getOutput('Arya'), the value of name is 'Arya', so the first condition is true, and it returns 'You are Arya'.
getOutput('John'); // 
when calling getOutput('John'), the value of name is 'John', so the second condition is true, and it returns 'You are John'.
getOutput(); // 
calling getOutput() without passing any argument, the default value of name is undefined. Since neither of the conditions is true, it returns the default message 'Who are you'.


What will be the output of the following code given below? Explain the reason?


Can a function have multiple return statement? Give one example if possible and explain the reason.

// Yes, A function have multiple return statement. 

function isEven(number) {
  if (number % 2 === 0) {
    return true; 
  } else {
    return false; 
  }
}

In this example, the isEven function takes a parameter number and checks if it's even. If number is divisible by 2 without any remainder, the function returns true, indicating that the number is even. If number is not divisible by 2, the function returns false, indicating that the number is odd.
//

What is the difference between for loop and while loop. What are the different place you can use them? Explain with example.

// The main difference between a for loop and a while loop is in their syntax and how they control the loop execution

For loop
for loop is used when the number of iteration is known or infinite. the loop continous until the condition is false. for eg.

for (i = 1; i <= 10; i++){
    console.log(i)
} // output 1,2,3,4.....10

while loop
while loop is used when the number of iteration is unknown or undefinite. It's generally used when you don't know in advance how many times you need to iterate, and you want to continue until a certain condition is met.

let i = 0;
while (i < 5){
  console.log(i);
  i++;
} // output 0,1,2..5