# READ CLASS 04 CLASSES and OBJECTS

- Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

- You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class.

- To access a function inside of an object you use notation similar to accessing a variable:


`class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.function()`

## Thinking Recursively in Python

- Santa Claus has a list of houses he loops through. He goes to a house, drops off the presents, eats the cookies and milk, and moves on to the next house on the list.

- The function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

- Subproblems must eventually become so simple that they can be solved without further subdivision. This is the base case.

- To maintain state during recursion you have to either:

1.Thread the state through each recursive call so that the current state is part of the current call’s execution context.

2.Keep the state in global scope.

- A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure.

- Python doesn’t have support for tail-call elimination. As a result, you can cause a stack overflow if you end up using more stack frames than the default call stack depth.