# Reading 2
## In Tests We Trust — TDD with Python

The author gavve an intro about TDD with Python with somme examples: 
Refactoring and unit tests.

Unit tests:mainly check the behaviour of our code. 

The freela: 
what is the smaller test against functions we have? 
in this example : given a name, return a gender.

what to take into consideration: 
1-Test name: "should follow the same name of module name".
2-structure: 
Arrange: organize the data (input);
Act: execute the code being tested (exercise the behaviour);
Assert: check if the result (output) is the same as you were expecting.

pytest can be used to test it. 

The Cycle: using baby steps.
* 🆘 Write a unit test and make it fail 
✅ Write the feature and make the test pass! 
🔵 Refactor the code 

TDD is not about the money/tests: its about software design first.

Empty name should be aslo considered.

in concolusion: 
the author concluded :
* Craft the software design first
* Reliable code.
* Practice!


# What does the if __name__ == “__main__”: do?

 "If this file is being imported from another module, __name__ will be set to the module’s name"

"A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended"

there are four advantages to use teh following code as per the author: 
--------------------------------------
Test using testing __name__ variable.

if __name__ == "__main__":
    my_function()
 
import myscript
 
myscript.my_function()
---------------------------------------
Advantages :
* The module is being run standalone 
* Import that script as a module in another script, the __name__ is set to the name of the script/module.
* Python files can act as either reusable modules, or as standalone programs.
* if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.
  

 # Recursion :
 Def: "The process in which a function calls itself directly or indirectly"

 the author has show different aprroches can be used to solve a Mathematical delima using "Recursive adding"

  the idea is to break your problem into smaller ones, add a base condition.

  stack overflow error occurs when the memory is exhausted.

Direct and indirect recursion:
Direct => calls same function. 
Indirect=> calls another function.

Tailed and non-tailed recursion:
"A recursive function is tail recursive when recursive call is the last thing executed by the function"

Memory: 
When any function is called => main(), memory is allocated on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated.

What are the disadvantages of recursive programming over iterative programming? 
* The recursive program has greater space requirements than iterative program
* Greater time requirements

What are the advantages of recursive programming over iterative programming? 
* Recursion is a clean and simple way to write code.


The author gave a lot of examples that you can refer to here : https://www.geeksforgeeks.org/recursion/


