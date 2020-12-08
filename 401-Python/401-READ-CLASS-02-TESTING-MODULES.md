# Testing Modules

## Unit tests and TDD

- Unit tests are pieces of code to excercise the input, output and behavior of the code.

1. `Test name` the tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.

- The test file name should follow the same name of module name.

ex. gender.py, test_gender.py.

- A convention widely used is the AAA: Arrange, Act and Assert.

- `Arrange`: you need to organize the data needed to execute that piece of code (input);

- `Act`: here you will execute the code being tested (exercise the behaviour);

- `Assert`: after executing the code, you will check if the result (output) is the same as you were expecting.

### The Cycle

1. Write a unit test and make it fail.

2. Write the feature and make the test pass!

3. Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)

- The greatest advantage about TDD is to craft the software design first.

- Your code will be more reliable: after a change you can run your tests and be in peace.

## Recursion

- The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function.

### What is the difference between direct and indirect recursion?

- A function `fun()` is called direct recursive if it calls the same function `fun()`.

- A function `fun()` is called indirect recursive if it calls another function say `fun_new()` and `fun_new()` calls `fun()` directly or indirectly.