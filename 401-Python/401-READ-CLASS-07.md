# Read: Class 07 Game of Greed 2


## Modifying Behavior of Python Scope

### The Global Statement

- You already know that when you try to assign a value to a global name inside a function, you create a new local name in the function scope. To modify this behavior, you can use a global statement.

- With this statement, you can define a list of names that are going to be treated as global names.

- `global` counter  # Declare counter as global

- The use of global is considered bad practice in general. 

### The nonlocal Statement

- Similarly to global names, nonlocal names can be accessed from inner functions, but not assigned or updated. 

## Built in Functions

- `globals()` is a built-in function that returns a reference to the current global scope or namespace dictionary. This dictionary always stores the names of the current module.

- This means that if you call `globals()` in a given module, then you’ll get a dictionary containing all the names that you’ve defined in that module, right before the call to `globals()`.

- You can use the `globals()` dictionary just like you would use any regular dictionary.

- You can also perform regular subscription operations over globals() by using square brackets like in globals()['name'].

- `locals()` is a function that updates and returns a dictionary that holds a copy of the current state of the local Python scope or namespace.

- If you call `locals()` in the global Python scope, then you’ll get the same dictionary that you would get if you were to call `globals()`.