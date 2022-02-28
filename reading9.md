# Functional Programming Concepts

source: https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2a 

### What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

### What is a pure function and how do we know if something is a pure function?

It's programming concepts.
 - It returns the same result if given the same arguments (it is also referred as deterministic)
 - It does not cause any observable side effects


### What are the benefits of a pure function?

It is easier to test.

### What is immutability?

When data is immutable, its state cannot change after it’s created.

### What is Referential transparency?

If a function consistently yields the same result for the same input, it is referentially transparent.


# Node JS Tutorial for Beginners #6 - Modules and require()

source: https://www.youtube.com/watch?v=xHLd36QoS4k

### What is a module?

A seperate set of code with a specific function.

### What does the word ‘require’ do?

lets you use module where ever you want to use it.

### How do we bring another module into the file that we are working in?
 
Use require to bring in a module.
require('./file name')  

### What do we have to do to make a module available?

Use export to make the modules available.
module.exports = name of what you want to export.
