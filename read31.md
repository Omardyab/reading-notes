# Reading 10
What is a ‘call’? A call is when you invoke a function, meaning it triggers the behavior or calculation of the function to happen

How many ‘calls’ can happen at once? Only one function at a time, since Javascript is single-threaded

What does LIFO mean? Last in, First out

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

first function = {
  console.log(`Hello from first`)
} 

second function = {
  // calling first fucntion
  first();
}
// invoking second funtion which trigger the first
second();
What causes a Stack Overflow? Stack over flow occurs when a loop is created through invoking a function, when it continues to call on it's self, never resolving to a solution of final return

Errors & Debugging
What is a ‘refrence error’?

We get refernce errors most commonly when we try to use variables that are not delcared
What is a ‘syntax error’?

A syntax error is when the running the code cannot be parsed due to syntax
What is a ‘range error’?

Range errors occur when we try and manipulate an object with some kind of legnth and is given an invalid length
What is a ‘type error’?

Type errors occur when the code is expecting a certain data type in order to process it self, but does not recieve the data type expected.
What is a breakpoint?

A break point is a point at which code stops when a condition is met
What does the word ‘debugger’ do in your code?

runs code up to a determined break point in order to test specific functions