# READ CLASS 08

## List Comprehensions in Python

- Consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. 

- The expressions can be anything, meaning you can put in all kinds of objects in lists.

`new_list = [expression(i) for i in old_list if filter(i)]`

`new_list` - The new list (result)

`expression(i)` - Expression is based on the variable used for each element in the old list.

`for i in old_list` - The word for followed by the variable name to use, followed by the word in the
old list.

`if filter(i)` - Apply a filter with an If-statement.

### Using list comprehension in functions

def double(x):
  return x*2

`[double(x) for x in range(10)]`