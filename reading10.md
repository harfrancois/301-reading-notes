# Understanding the JavaScript Call Stack

source: https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4

### What is a ‘call’?

function invocation

### How many ‘calls’ can happen at once?

Only one call at a time

### What does LIFO mean?

Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

1. When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
2. secondFunction() then calls firstFunction()which is pushed into the stack.
3. firstFunction() returns and prints “Hello from firstFunction” to the console.
4. firstFunction() is pop off the stack.
5. The execution order then move to secondFunction().
6. secondFunction() returns and print “The end from secondFunction” to the console.
7. secondFunction() is pop off the stack, clearing the memory.

### What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

# JavaScript error messages

source: https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c

### What is a ‘reference error’?

Variable not yet declared.

### What is a ‘syntax error’?

You have something that cannot be parsed in terms of syntax.

### What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length

### What is a ‘type error’?

The types (number, string and so on) you are trying to use or access are incompatibl

### What is a breakpoint?
A point where the program stops when the statement evaluates to true.

### What does the word ‘debugger’ do in your code?

Let's you can see the “history” before reaching that breakpoint.