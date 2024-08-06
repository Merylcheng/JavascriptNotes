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
