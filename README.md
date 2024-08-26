### 08/26/24 Phase 1 Lecture: Functions & Scope

Here is the code that we covered today

```
/*
Expectations for lecture
1. You know what variables are
2. You know what datatypes are: strings / integers / booleans
3. You know what comments are

Agenda

Functions
- What is a function?
  - Functions are our verbs, it consist of a block of code
- Function Syntax
- Code Block
- Calling a Function
- console.log vs return
- arguments

Scope
- Global Scope
- Function Scope
- Block Scope

Callback Functions
- Functions definitions vs calling a function
- Passing in function definitions
- Calling the passed in function inside of another function
*/

// function greet() {
//   console.log('Hello! How are you?')
// }

// greet()

// function addTwoNums(num1, num2=1) {
//   return num1 + num2
// }

// let addTwoNums = function(num1, num2=1) {
//   return num1 + num2
// }

// let addTwoNums = (num1, num2=1) => num1 + num2

// let result = addTwoNums(3) + addTwoNums(4, 1)

// console.log('the result of add two nums is: ' + result)

// global scope, or global variable
// let name = "Bob"

// function greet(name) {
//   name = "Sam"
  
//   if(true) {
//     if(true){
//     const name = "Sarah"
      
//     }
//     console.log("inside the if condition's code block: " + name)
//   }
  
//   console.log("inside the function greet: " + name)
// }


// greet(name)

// console.log("global scope: " + name)

function doMath(num1, num2, callback) {
  let result = callback(num1, num2)
  console.log(console.log('doMath result is: ' + result))
}

const addTwoNums = function(num1, num2) {
  return num1 + num2
}

const subtractTwoNums = function(num1, num2) {
  return num1 - num2
}

doMath(1, 3, addTwoNums)
doMath(3, 1, subtractTwoNums)
doMath(2, 2, (num1, num2) => num1 * num2)
doMath(2, 2, function(num1, num2) {
  return num1 / num2
})
```
