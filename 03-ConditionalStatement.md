# Conditional Statements

if we are tired, we go to bed, otherwise, we wake up and start our day.

These if-else decisions can be modeled in code by creating conditional statements. A conditional statement checks a specific condition(s) and performs a task based on the condition(s).

We’ll be covering the following concepts:

if, else if, and else statements
comparison operators
logical operators
truthy vs falsy values
ternary operators
switch statement

## if

eg
let sale = true;
if (sale) {
console.log('Time to buy!')
}

let sale = false;
if (sale) {
console.log('Time to buy!')
}

ans:
Time to buy!

nothing will print out cos its false

## if ...else

eg
let sale = true;

sale = false;

if(sale) {
console.log('Time to buy!');
} else {
console.log('Time to wait for a sale.');
}

ans:
Time to wait for a sale.

if (false) {
console.log('The code in this block will not run.');
} else {
console.log('But the code in this block will!');
}

// Prints: But the code in this block will!

In the example above, the else statement:

Uses the else keyword following the code block of an if statement.
Has a code block that is wrapped by a set of curly braces {}.
The code inside the else statement code block will execute when the if statement’s condition evaluates to false.
if...else statements allow us to automate solutions to yes-or-no questions, also known as binary decisions.

## Comparison Operators

When writing conditional statements, sometimes we need to use different types of operators to compare values.
Here is a list of some handy comparison operators and their syntax:

Less than: <
Greater than: >
Less than or equal to: <=
Greater than or equal to: >=
Is equal to: ===
Is not equal to: !==

10 < 12 // Evaluates to true

\*\* TIPS
It can be helpful to think of comparison statements as questions. When the answer is “yes”, the statement evaluates to true, and when the answer is “no”, the statement evaluates to false. The code above would be asking: is 10 less than 12? Yes! So 10 < 12 evaluates to true.

let hungerLevel = 7
if (hungerLevel > 7 ) {
console.log('Time to eat!')
}
else {
console.log('We can eat later!')

Ans:
We can eat later!
}

## Logical Operators

Working with conditionals means that we will be using booleans, true or false values.

There are three logical operators:

the and operator (&&)
the or operator (||)
the not operator, otherwise known as the bang operator (!)
When we use the && operator, we are checking that two things are true:

if (stopLight === 'green' && pedestrians === 0) {
console.log('Go!');
} else {
console.log('Stop');
}

When using the && operator, both conditions must evaluate to true for the entire condition to evaluate to true and execute. Otherwise, if either condition is false, the && condition will evaluate to false and the else block will execute.

If we only care about either condition being true, we can use the || operator:

if (day === 'Saturday' || day === 'Sunday') {
console.log('Enjoy the weekend!');
} else {
console.log('Do some work.');
}

When using the || operator, only one of the conditions must evaluate to true for the overall statement to evaluate to true. In the code example above, if either day === 'Saturday' or day === 'Sunday' evaluates to true the if‘s condition will evaluate to true and its code block will execute. If the first condition in an || statement evaluates to true, the second condition won’t even be checked. Only if day === 'Saturday' evaluates to false will day === 'Sunday' be evaluated. The code in the else statement above will execute only if both comparisons evaluate to false.

The ! not operator reverses, or negates, the value of a boolean:

let excited = true;
console.log(!excited); // Prints false

let sleepy = false;
console.log(!sleepy); // Prints true

Essentially, the ! operator will either take a true value and pass back false, or it will take a false value and pass back true.

## Truthy and Falsy

non-boolean data types, like strings or numbers, are evaluated when checked inside a condition.

Sometimes, you’ll want to check if a variable exists and you won’t necessarily want it to equal a specific value — you’ll only check to see if the variable has been assigned a value.

let myVariable = 'I Exist!';

if (myVariable) {
console.log(myVariable)
} else {
console.log('The variable does not exist.')
}

So which values are falsy— or evaluate to false when checked as a condition? The list of falsy values includes:

0
Empty strings like "" or ''
null which represent when there is no value at all
undefined which represent when a declared variable lacks a value
NaN, or Not a Number
Here’s an example with numbers:

let numberOfApples = 0;

if (numberOfApples){
console.log('Let us eat apples!');
} else {
console.log('No apples left!');
}

// Prints 'No apples left!'

The condition evaluates to false because the value of the numberOfApples is 0. Since 0 is a falsy value, the code block in the else statement will run.

EG
Say you have a website and want to take a user’s username to make a personalized greeting. Sometimes, the user does not have an account, making the username variable falsy. The code below checks if username is defined and assigns a default string if it is not:

let username = '';
let defaultName;

if (username) {
defaultName = username;
} else {
defaultName = 'Stranger';
}

console.log(defaultName); // Prints: Stranger

If you combine your knowledge of logical operators you can use a short-hand for the code above. In a boolean condition, JavaScript assigns the truthy value to a variable if you use the || operator in your assignment:

let username = '';
let defaultName = username || 'Stranger';

console.log(defaultName); // Prints: Stranger

Because || or statements check the left-hand condition first, the variable defaultName will be assigned the actual value of username if it is truthy, and it will be assigned the value of 'Stranger' if username is falsy. This concept is also referred to as short-circuit evaluation.

## Ternary Operator

use a ternary operator to simplify an if...else statement.

Take a look at the if...else statement example:

let isNightTime = true;

if (isNightTime) {
console.log('Turn on the lights!');
} else {
console.log('Turn off the lights!');
}

We can use a ternary operator to perform the same functionality:

isNightTime ? console.log('Turn on the lights!') : console.log('Turn off the lights!');

In the example above:

The condition, isNightTime, is provided before the ?.
Two expressions follow the ? and are separated by a colon :.
If the condition evaluates to true, the first expression executes.
If the condition evaluates to false, the second expression executes.

let stopLight = 'yellow';

if (stopLight === 'red') {
console.log('Stop!');
} else if (stopLight === 'yellow') {
console.log('Slow down.');
} else if (stopLight === 'green') {
console.log('Go!');
} else {
console.log('Caution, unknown!');
}

The else if statements allow you to have multiple possible outcomes. if/else if/else statements are read from top to bottom, so the first condition that evaluates to true from the top to bottom is the block that gets executed.

In the example above, since stopLight === 'red' evaluates to false and stopLight === 'yellow' evaluates to true, the code inside the first else if statement is executed. The rest of the conditions are not evaluated. If none of the conditions evaluated to true, then the code in the else statement would have executed.

## MAGIC EIGHT BALL PROJ

const userName = 'Jane'

console.log('Hello!')

const userQuestion = 'Do you like to study?'
console.log( userName, userQuestion )

let randomNumber = Math.floor(Math.random() \*3)
if (randomNumber === 0) {
console.log(eightBall)
}
if (randomNumber === 1) {
console.log('decide')
}
if (randomNumber === 2) {
console.log('hazy')
}
if (randomNumber === 3 ){
console.log('predict')
}

let eightBall = 'BINGO'

# FUNCTIONS
