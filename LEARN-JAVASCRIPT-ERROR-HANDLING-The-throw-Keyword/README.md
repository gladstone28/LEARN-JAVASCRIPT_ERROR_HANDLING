Lesson link:

https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-front-end-development/tracks/fscj-22-javascript-syntax-part-iii/modules/wdcp-22-learn-javascript-syntax-error-handling-f3582f01-f40d-4726-aea0-4ea8ebd08eec/lessons/error-handling/exercises/throw

### LEARN JAVASCRIPT: ERROR HANDLING

## The throw Keyword

Creating an error doesn’t cause our program to stop — remember, an error must be thrown for it to halt the program.

To throw an error in JavaScript, we use the throw keyword like so:
```
throw Error('Something wrong happened');
// Error: Something wrong happened
```
When we use the throw keyword, the error is thrown and code after the throw statement will not execute. Take for example:
```
throw Error('Something wrong happened');
// Error: Something wrong happened

console.log('This will never run');
```
After throw Error('Something wrong happened'); is executed and the error object is thrown, the console.log() statement will not run (just like when a built-in JavaScript error was thrown!).

In the next lesson we will cover how to handle an error so that the rest of our code can run!


### Instructions
Checkpoint 1 Passed
1. Use the throw keyword to throw an error with the message 'Username or password does not match'

After you clear this checkpoint, try adding some code after your throw statement. Also, try to throw a new error and other data types to see what happens!
Hint

To use the throw keyword, use the following syntax:
```
throw Error('Helpful message to pinpoint what went wrong!');
```

Or
```
throw new Error('Helpful message to pinpoint what went wrong!');
```
