#  Reading 24: Hash table

- A hash table is a data structure that is used to store information so the information in the hash table basically has two main components so it's going to have some sort of key and then it's going to have some sort of value or some sort of record, so basically a key could be something like for instance my name and the value could be something like my phone number, so we could basically create a hash table to store a bunch of people's phone numbers.

- Hash table it's a way that we can implement an associative array and so we're basically going to map this key to this value here and at the heart of a hash table we're basically just going to have this array structure.

- We're basically going to have a hash function and so what the hash function is going to do is it's
going to look at a certain key and then it's going to evaluate that key and it's going to spit out some sort of index number and it's going to tell us what location in the array to store this information, so for example we'll just go ahead and just write this out so our hash function is going to take a key value and as a result it's going to give us an index number so for example we could do hash and then as the argument we could enter my name, my name could be the key and then we could just say that our hash function evaluated this key and it said ok that in index three for instance.

- In index three and the way the hash function is written is that every time you enter that key if it's the same key it's going to spit out the same index number so every time I enter myname into my hash function I should get the index number of three so we could just represent myname as a circle so we'll just go ahead and put "O" circle is going to represent my name and my phone number and where it is located in the hash table so:

        Ohash(myname)=> 3

- For another person you can use square or diamond.

- If we want to add another person and  we find out that their hash value ends up being three.  we will linked list that index(chaning)

        Hash(person) => 1
        it will look in that index, and if we have some channing we will look into that when there is a collision. 
