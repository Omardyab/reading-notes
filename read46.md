# Reading 10: Stacks and Queues

# What is stack? 
*  Stack: This is a special case of linked list, instead of a head you will have top
in stack you are only able to insert at the top using push. 

* items can be added/removed to/from the top.
pop to remove an item from top.
peek view a value from top
isEmpty return True only when stack is empty

## Two main concepts in stack: 

* FILO meaning: 
               
            First in Last Out.
            First item added last to be removed

* LIFO meaning: 
            
            Last Out first out the oppopsite

* Using Push=> Node on stack is O(1)
	     Top should be reassigned to the new node once added.
* Using Pop=> Node on stack is O(1)
	    Top should be reassigned to the next node once removed.
* Using Peek=> inspecting or viewing the top Node od your stack
	     no re-assigning

### its more restriceted but this due to performance and complexity. 

# What is a Queue? 
FIFO: 
         
         First In First Out
         First item in the queue, your first to be out

LILO:   
        Last In Last Out. 
        last item in the queue, your last to be out

* Enqueue=> front/Rear
  
           To add a node 
           change rear.next 
* Dequeue=>
 
       Remove an item (front)  
	   change front to next
* Peek=> 
  
       inspecting or viewing front node


