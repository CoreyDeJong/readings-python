## Dunder Methods
- As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”
- constructor = __init__
- Length  = def __len__(self):
- Slice =  __getitem__ method which allows you to use Python’s list slicing syntax: obj[start:stop].
- __repr__: The “official” string representation of an object. This is how you would make an object of the class. The goal of __repr__ is to be unambiguous.
- __str__: The “informal” or nicely printable string representation of an object. This is for the enduser.
- Iteration: __len__, __getitem__, __reversed_
- Operator Overloading for Comparing Accounts: __eq__, __lt__
- Operator Overloading for Merging Accounts: __add__
- Callable Python Objects: __call__
- To iterate over transactions in reversed order you can implement the __reversed__ special method
- Context Manager Support and the With Statement: __enter__, __exit__

## Iterators
- instances of this Repeater class will repeatedly return a single value when iterated over
- Iterators provide a sequence interface to Python objects that’s memory efficient and considered Pythonic. Behold the beauty of the for-in loop!
- To support iteration an object needs to implement the iterator protocol by providing the __iter__ and __next__ dunder methods.
- Class-based iterators are only one way to write iterable objects in Python. Also consider generators and generator expressions.

## Generators
 - generators produce a series of values
 - The yield statement allows you to temporarily suspend execution of a generator function and to pass back values from it.
 - next() will run the generator at each sequence until the generator has been completed
 - list() will call next every time in one instance to show all the occurrences of next.












