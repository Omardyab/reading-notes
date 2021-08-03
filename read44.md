# Reading 8: List Comprehensions in Python

# List Comprehensions : 
def: "It consists of brackets containing an expression followed by a for clause, then
zero or more for or if clauses. The expressions can be anything, meaning you can
put in all kinds of objects in lists."

here was a given example and how to make  list comprehension: 

    new_list = []
    for i in old_list:
        if filter(i):
            new_list.append(expressions(i))

    new_list = [expression(i) for i in old_list if filter(i)]

    Mainly : 
    we have an existing list that has data then we access the list and do an action (accessing and manipulating) transform it to a new list


another example (Squares): 
   
    squares = []
    for x in range(10):
    squares.append(x**2)
that is the same as : 

    squares = [x**2 for x in range(10)]

another example (filter): 

    fh = open("test.txt", "r")
    result = [i for i in fh if "line3" in i]
    print result

## Using list comprehension in functions
 
### Examples on how to use functions : 
    def double(x):
    return x*2
    >>> print double(5)
    10

    >>> [double(x) for x in range(10)]
    print double
    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
    # with conditions:
    >>> [double(x) for x in range(10) if x%2==0]
    [0, 4, 8, 12, 16]

    # with more arguments:

    >>> [x+y for x in [10,30,50] for y in [20,40,60]]
    [30, 50, 70, 50, 70, 90, 70, 90, 110]


* more examples: https://www.pythonforbeginners.com/basics/list-comprehensions-in-python#htoc-syntax
