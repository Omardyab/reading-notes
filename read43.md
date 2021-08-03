# Reading 7: global and nonlocal names

# How to use the Random Module in Python:
* Global names can be accessed anywhere in my code.
* Local names can be accessed (or edited) inside the function they were created.
* nonlocal names can be modified or updated, only accessed 

### Such standards can be modified within those two keywords: 
    1- global
    2- nonlocal

## global statement: 
* What: define a list to be global names.
* How: global followed by the name (list of names)
   the author shows the following example in which a global name can be updated inside your function : 
   >>> counter = 0  # A global name
    >>> def update_counter():
...     global counter  # Declare counter as global
...     counter = counter + 1  # Successfully update the counter 

* It's better to avoid lazy global names it can end up with an error if you did not call the function where you have the global name.  
Generate random numbers by providing access to functions.


## The nonlocal Statement

* What: define a list to be nonlocal.
* How: nonlocal followed by the name or more separated by commas.
* The author shows the following example in which a nonlocal name can be updated inside your function :
   >>> def func():
...     var = 100  # A nonlocal variable
...     def nested():
...         nonlocal var  # Declare var as nonlocal
...         var += 100
...
...     nested()
...     print(var)
...
>>> func()
200

* nonlocal cant be used outside of your function (not in global scope nor local scope)
*  you cant use nonlocal to create lazy nonlocal names (raises a SyntaxError)