# Reading 3

React Lists & Keys
What does .map() return?

[2,4,6,8,10]
If I want to loop through an array and display each value in JSX, how do I do that in React?

By using JavaScript .map(), then returning the result to a varible that is then placed in an HTML element that is rendered using ReactDOM
Each list item needs a unique?

id
What is the purpose of a key?

Key helps React identify items that have been changed, added, or removed.
The Spread Operator
What is the spread operator?

*In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

List 4 things that the spread operator can do.

Using Math functions Using an array as arguments Adding an item to a list Adding to state in React

Give an example of using the spread operator to combine two arrays.

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
Give an example of using the spread operator to add a new item to an array.
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
Give an example of using the spread operator to combine two objects into one.
const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}
const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }
The Spread Operator
In the video, what is the first step that the developer does to pass functions between components?

assigned a variable within the increment funtction and assigned it the value of the object instance running through a .map() function
In your own words, what does the increment function do?

The increment functions passes through an array of objects and looks for a name. If the name matches it adds 1 to the value of the count property, then it updates the state of the component.
How can you pass a method from a parent component into a child component?

you create an object with a refernce to the function with in the parent ex: object={this.functionFromParent}, giving access to the component to the parents function
How does the child component invoke a method that was passed to it from a parent component?

This.props.function()
