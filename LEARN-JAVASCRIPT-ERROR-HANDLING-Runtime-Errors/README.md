


### LEARN JAVASCRIPT: ERROR HANDLING

## Runtime Errors

Errors contain useful messages that tell us why our program isn’t working or why the error was thrown. When an error is thrown, our program stops running and the console displays the error message in red text like so:

![](./error_diagram.svg)

When we execute code and a line of code throws an error, that error is referred to as a runtime error. In JavaScript, there are built-in error objects that have a name and message property which tell us what went wrong. Examples of built-in runtime errors include:

- ReferenceError: when a variable or function cannot be found.
- TypeError: when a value is not a valid type, see the example below:
```
const reminder = 'Reduce, Reuse, Recycle';
reminder = 'Save the world';
// TypeError: Assignment to constant variable.
console.log('This will never be printed!');
```
In the example above, when we try to reassign a constant variable reminder, the TypeError is thrown. Code that is written after a thrown runtime error will not be evaluated, so the console.log() statement will not be evaluated.

Let’s see for ourselves what happens when a runtime error is thrown.


### Instructions
Checkpoint 1 Passed
1. In main.js, we have a function throwError() that will throw a ReferenceError. There are also two console.log() statements, one at the top of the file and one at the bottom.

Call throwError() below the comment that indicates to call it. Observe what code runs and what code doesn’t.

Make sure you call throwError() before the second console.log() statement. If done correctly, the first console.log() statement will print while the second console.log() statement won’t.
