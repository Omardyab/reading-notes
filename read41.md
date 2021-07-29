# Reading 5: Linked Lists

* linked lists is a very simple data structure.
It's essentially just a sequence of elements, where each element links to the next
element which links the next element. 
A linked list can contain pretty much anytype of data, strings, characters, numbers, the elements can be unsorted or sorted,they can contain duplicate elements or all unique elements. One of the things
that distinguishes a linked list from an array which shares many of the same
properties is that in the array elements are indexed. That is, if you want to get
to the fourth element you can just instantly do that. In a linked list
though you have to start with the head and work your way through until you get
to the fourth element, That takes linear time so it's quite a bit slower.
but why would anyone use such a data structure? Well the advantage of a linked list is
that insertions and deletions can be very quick. If you just want to insert an
element right to the beginning of the linked list, that can be done in constant
time. If you want to delete an element from the beginning of the linked list again
constant time. So that's very fast.

* If you want to append an element to the end of the linked list
that might require walking all the way through the linked list until you get
the very last element and then inserting the element there. That will take linear
time so it all depends on what you're looking for.
There's this alternate version called a doubly linked list. 
A doubly linked list is just like a singly linked list but in addition to each element
having a link to the next element, each element also links the previous element.
For certain operations that can be quite handy.
We just need a class node that takes in, has a next value, and a data, and then
add in a constructor.And set that value. 
Append is going to take in a data value and then it's going to have some pointer that starts off
at the current node so the head of the linked list and then it's going
to walk through the linked list until we get to the end of the linked list.
We're not at the end of the linked list as long as there's something after
it.

* If we prepend an element we're going to actually change
what the head node is. Now this makes a little bit of an issue because we could
have multiple places our code base that all link to the same head. But if we
change the head in one place
how does everybody else know that our head value changed? So the workaround for
this is rather than giving everybody an access to the head pointer directly, we
define a class linked list that's basically going to wrap our head. And
then the append method can go where it probably should have from the
beginning, which is in this linked list class. 
If the head is null,then create the head.
delete method deletes the first node that has a particular value.
if head is null, we know we just want to return immediately.
Now what delete with value is going to do is its going to walk through the linked list and it's going to stop one
before the element we want to delete. And then the very next
element you want to delete. So update my pointers to
work around it so my next pointer is going to be that deleted values next
pointer. 
First we have this current method that walks through the linked list.
And then we're going to walk through as long as we're not at the last element so
we don't want to run off the edge of the linked list.

* If current.next.data equals the data were trying to lead,in other words if the next value is the one you want to delete, then cut out that
next value. so then current.next will be  current.next.next.
So what this is doing is saying, okay, if the next value you want to delete, don't go
to the element, and just walk around it. Set my next pointer to be my next
pointer's next pointer so walk around it.  
 
