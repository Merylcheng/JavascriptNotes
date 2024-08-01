Variables

a variable is a container for a value. You can think of variables as little containers for information that live in a computer’s memory. Information stored in variables, such as a username, account number, or even personalized greeting can then be found in memory.

Variables also provide a way of labeling data with a descriptive name, so our programs can be understood more clearly by the reader and ourselves.

In short, variables label and store data in memory. There are only a few things you can do with variables:

1. Create a variable with a descriptive name.
2. Store or update information stored in a variable.
3. Reference or “get” information stored in a variable.

eg
var favouriteFood = 'pizza'
var numOfSlices = 8
console.log(favouriteFood)
console.log(numOfSlices)

ans:
pizza
8

## let

The let keyword signals that the variable can be reassigned a different value.
eg
let changeMe = true
changeMe = false
console.log(changeMe)

ans: false

you are not able to change const

## Mathematical Assignment Operators

use variables and math operators to calculate new values and assign them to a variable

let levelUp = 10;
let powerLevel = 9001;
let multiplyMe = 32;
let quarterMe = 1152;

// Use the mathematical assignments in the space below:
levelUp += 5
powerLevel -= 100
multiplyMe \*= 11
quarterMe /= 4

let x = 20;
x -= 5; // Can be written as x = x - 5
console.log(x); // Output: 15

// These console.log() statements below will help you check the values of the variables.
// You do not need to edit these statements.
console.log('The value of levelUp:', levelUp);
console.log('The value of powerLevel:', powerLevel);
console.log('The value of multiplyMe:', multiplyMe);
console.log('The value of quarterMe:', quarterMe);

ans:
15
The value of levelUp: 15
The value of powerLevel: 8901
The value of multiplyMe: 352
The value of quarterMe: 288

## The Increment and Decrement Operator

increment operator (++)  
The increment operator will increase the value of the variable by 1.

decrement operator (--).
The decrement operator will decrease the value of the variable by 1.

eg
let gainedDollar = 3;
gainedDollar++;
console.log(gainedDollar)

let lostDollar = 50;
lostDollar--;
console.log(lostDollar)

ans:
4
49

## String Concatenation with Variables

In previous exercises, we assigned strings to variables. Now, let’s go over how to connect, or concatenate, strings in variables.

The + operator can be used to combine two string values even if those values are being stored in variables:

eg
var favouriteAnimal = 'Misha'
console.log('My favourite animal: ' + favouriteAnimal)

ans:
My favourite animal: Misha

## String Interpolation

insert, or interpolate, variables into strings using template literals.

### a template literal is wrapped by backticks `

var myName = 'meryl'
var myCity = 'pasir ris'
console.log(`My name is ${myName}. My favourite city is ${myCity}.`);

ans:
My name is meryl. My favourite city is pasir ris.

## typeof operator

While writing code, it can be useful to keep track of the data types of the variables in your program. If you need to check the data type of a variable’s value, you can use the typeof operator.

The typeof operator checks the value to its right and returns, or passes back, a string of the data type.

eg
let newVariable = 'Playing around with typeof.';
console.log(typeof newVariable);
newVariable = 1
console.log(typeof newVariable);

ans:
string
number
