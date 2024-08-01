## Data types

are the classifications we give to the different kinds of data that we use in programming. In JavaScript, there are eight fundamental data types:

Number: Any number, including numbers with decimals: 4, 8, 1516, 23.42.
BigInt: Any number, greater than 253-1 or less than -(253-1), with n appended to the number: 1234567890123456n.
String: Any grouping of characters on your keyboard (letters, numbers, spaces, symbols, etc.) surrounded by single quotes: ' ... ' or double quotes " ... ", though we prefer single quotes. Some people like to think of string as a fancy word for text.
Boolean: This data type only has two possible values— either true or false (without quotes). It’s helpful to think of booleans as on and off switches or as the answers to a “yes” or “no” question.
Null: This data type represents the intentional absence of a value, and is represented by the keyword null (without quotes).
Undefined: This data type is denoted by the keyword undefined (without quotes). It also represents the absence of a value though it has a different use than null. undefined means that a given value does not exist.
Symbol: A newer feature to the language, symbols are unique identifiers, useful in more complex coding. No need to worry about these for now.
Object: Collections of related data.

The first 7 of those types are considered primitive data types. They are the most basic data types in the language. Objects are more complex, and you’ll learn much more about them as you progress through JavaScript. At first, eight types may not seem like that many, but soon you’ll observe the world opens with possibilities once you start leveraging each one. As you learn more about objects, you’ll be able to create complex collections of data.

## Arithmetic Operators

An operator is a character that performs a task in our code.

Add: +
Subtract: -
Multiply: \*
Divide: /
Remainder: %

## String Concatenation

Operators aren’t just for numbers! When a + operator is used on two strings, it appends the right string to the left string:
eg
console.log('Hello' + 'World')
HelloWorld

## Properties

When you introduce a new piece of data into a JavaScript program, the browser saves it as an instance of the data type. All data types have access to specific properties that are passed down to each instance.
The . is another operator! We call it the dot operator.
eg
console.log('Teaching the world how to code'.length)
30

## Methods -actions we can perform.

Data types have access to specific methods that allow us to handle instances of that data type. JavaScript provides a number of string methods.
eg
// Use .toUpperCase() to log 'Codecademy' in all uppercase letters
console.log('Codecademy'.toUpperCase());

// Use a string method to log the following string without whitespace at the beginning and end of it.
console.log(' Remove whitespace '.trim());

ans:
CODECADEMY
Remove whitespace

## Built-in Objects

if you wanted to perform more complex mathematical operations than arithmetic, JavaScript has the built-in Math object.
eg
console.log(Math.random()); // Prints a random number between 0 and 1

Math.floor() rounds the number down to the nearest whole number.

Math.ceil() returns the smallest integer greater than or equal to a decimal number.

Number object that checks if a number is an integer.

### TAKE NOTE THAT () BRACKETS WILL DO THE MOST INNER BRACKETS FIRST

console.log(Math.random());
console.log(Math.floor(Math.random() *100));
console.log(Math.floor(Math.random() *100));
console.log(Math.ceil(43.8));
console.log(Number.isInteger(2017))

ans:
0.40205016470000343
89
54
44
true
