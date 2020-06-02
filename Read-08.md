## List Comprehension
 - list comprehensions will result in a new list from evaluating the expression in the context of the for and if clauses which follow it. 
 ```py
 new_list = []
for i in old_list:
    if filter(i):
        new_list.append(expressions(i))
```
or 
```py
new_list = [expression(i) for i in old_list if filter(i)]
```
Example:
```py
list1 = [3,4,5]
 
multiplied = [item*3 for item in list1] 
 
print multiplied 
[9,12,15]
```

## Decorators
- Decorator is a function that takes another function and extends its behavior without modifiying the functions 