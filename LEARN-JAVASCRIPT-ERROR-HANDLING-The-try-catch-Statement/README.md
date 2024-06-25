Lesson link:

https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-front-end-development/tracks/fscj-22-javascript-syntax-part-iii/modules/wdcp-22-learn-javascript-syntax-error-handling-f3582f01-f40d-4726-aea0-4ea8ebd08eec/lessons/error-handling/exercises/try-catch-i


### LEARN JAVASCRIPT: ERROR HANDLING

## The try...catch Statement

Up to this point, thrown errors have caused our program to stop running. But, we have the ability to anticipate and handle these errors by writing code to address the error and allow our program to continue running.

In JavaScript, we use try...catch statement to anticipate and handle errors. Take a look at example below:

try {
  throw Error('This error will get caught');
} catch (e) {
  console.log(e);
}
// Prints: This error will get caught

console.log('The thrown error that was caught in the try...catch statement!');
// Prints: 'The thrown error that was caught in the try...catch statement!'

Now, let’s break down what happened in the try...catch statement above:

- We have code that follows try inside curly braces {} known as the try block.
- Inside the try block we insert code that we anticipate might throw an error.
- Since we want to see what happens if an error is thrown in the try block, we throw an error with the message 'This error will get caught'.
- Following the try block is the catch statement which accepts the thrown error from the try block . The e represents the thrown error.
- The curly braces that follow catch(e) is known as the catch block and contains code that executes to handle the error.
- Since the error is caught, our console.log() after the try...catch statement prints 'The thrown error that was caught in the try...catch statement!'.

Generally speaking, in a try...catch statement, we evaluate code in the try block and if the code throws an error, the code inside the catch block will handle the error for us. The provided example just showcases how a try...catch statement works because we know an error is being thrown. Let’s first practice writing our own try...catch statement and afterwards we will go over a more practical usage of try...catch.


### Instructions
Checkpoint 1 Passed
1. Create a try...catch statement that doesn’t have any code in the try block or the catch block. Make sure to use e as the error object.

The syntax for a try...catch statement:
```
try {
  // try block code
} catch (e) {
  // catch block code
}

```

2. In the try block, throw an error using the Error() function and pass into Error() a string containing a message of your choice!

Hint

To throw an error, use the throw keyword and the Error function:
```
throw Error('error message goes here');

```

Make sure you’re adding the code within the try block:
```
try {
  throw Error('error message goes here');
} catch (e) {
  // catch block code
}

```
