# How to use Random Module
### This will output either 1, 2, 3, 4 or 5. 
import random
print random.randint(0, 5)

#a random number between 0 and 100:
import random
random.random() * 100

### Generate a random value from the sequence sequence.
random.choice( ['red', 'black', 'green'] ).

#The shuffle function, shuffles the elements in list in place, so they are in a
random order.
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)

### Generate a randomly selected element from range(start, stop, step)
### Template
random.randrange(start, stop[, step])

### Example
import random
for i in range(3):
    print random.randrange(0, 101, 5)

# Dependency Injection
- dependency is when one class relies on methods within another class
- transferring the task of creating the object to someone else and directly using the dependency is called dependency injection