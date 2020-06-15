## Hash Table
- Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
- hash function takes a key and returns an integer
- A hash table is a data structure that is used to store keys/value pairs. It uses a hash function to compute an index into an array in which an element will be inserted or searched
- chaining is when you have multiple key/value pairs off of the same index of the hash table, the chain will make the connection between these two key/value pairs using a linked-list
- A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table.
- Hashing is implemented in two steps:
    - An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
    - The element is stored in the hash table where it can be quickly retrieved using hashed key.
- The load factor tells us something about how full the hash table is.