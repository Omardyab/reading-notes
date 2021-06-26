# Reading 4
React Docs - Forms
What is a ‘Controlled Component’?
A Controlled Component is when a react component that renders a form, it also controls what occurs in that form on another user input. This input form element’s value is controlled by react in this way is called a Controlled Component.

Should we wait to store the user's responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?
We should update the state with the responses asap when entered.

How do we target what the user is entering if we have an event handler on an input field?
If we have an event handler in the input field we can target what the user is entering by setting the value of the input field to sync to the desired state to be changed, then the event handler updates that state when a change occurs.

The Conditional (Ternary) Operator Explained
Why would we use a ternary operator?
The ternary operator works like a if else statement.

Rewrite the following statement using a ternary statement:
if(x===y){ console.log(true); } else { console.log(false); }

let result = (x === y ? console.log(true) : console.log(false));