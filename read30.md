# Reading 9
What is functional programming?

functional programming is a programming paradigm -- a style of building the structure and elements of computer programs -- that treats computation as the evaluation of mathermatical functions and avoids chaging-state and mutable data -- wikipedia

What is a pure function and how do we know if something is a pure function?

A pure function retrurns the same result when given the same arugments, aka deterministic, and does not cause any side effect. An example of a impure function, would be a function that relies on global object that was not passed down as a parameter of the function
What are the benefits of a pure function?

A pure functions does not alter variables out side of it self, therefore the process of it's function cannot influence or change other functions
What is immutability?

'unchanging over time or unable to change',

Data with a state that cannot change after it's creation is what is known as immutable data. If it's necessary to change an immutable object, you would rather then have to craate a new object with a new value.
What is Referential transparency?

A function that awalays returns the same results when given the same parameters
Modules and require()
What is a module?

Module is basically another javascript file.
What does the word ‘require’ do?

Require creates a global object, by using a path to the module or other javascript file
How do we bring another module into the file the we are working in?

We use module.exports = x;
What do we have to do to make a module available?

We have to store it to a variable ex: 'let function = require(./module-with-function)'