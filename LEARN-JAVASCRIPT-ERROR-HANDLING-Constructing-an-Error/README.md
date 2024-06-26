Lesson link:

https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-front-end-development/tracks/fscj-22-javascript-syntax-part-iii/modules/wdcp-22-learn-javascript-syntax-error-handling-f3582f01-f40d-4726-aea0-4ea8ebd08eec/lessons/error-handling/exercises/error-construction

### LEARN JAVASCRIPT: ERROR HANDLING

## Constructing an Error

JavaScript errors are objects that have a name and message property. Previously, we’ve seen how built-in errors alert us about common mistakes in our code. But, what if we need an error message that isn’t covered by the built-in errors? Let’s say we need to inform a user that a string passed in as an argument is too short with a custom message. Such a message isn’t covered by a built-in error, but we could use the Error function to make our own error object with a message that is unique to our program!
```
console.log(Error('Your password is too weak.'));
// Prints: Error: Your password is too weak.
```
The Error function takes an argument of a string which becomes the value of the error’s message property. In the code snippet above, we used the Error function to create an error object that has the message 'Your password is too weak.'.

You might also see errors created with the new keyword. Both methods will lead to the same functionality. Take a look:
```
console.log(new Error('Your password is too weak.'));
// Prints: Error: Your password is too weak.
```
Keep in mind that creating an error is not the same as throwing an error. A thrown error will cause the program to stop running. We’ll cover how to throw our created errors in the next exercise!


### Instructions

Checkpoint 1 Passed

1. At the top of main.js add a console.log() that prints an error with the message 'User missing name'.

After running the code, take note of the console.log() at the bottom of main.js and if that line of code still runs.

The argument passed to the Error() function becomes the message property of the new error. You may use the Error() function create the error object or use the new keyword with the Error().
```
console.log(Error('Message goes here'));
// OR
console.log(new Error('Message goes here'));
```
