# Read: 10 - The Call Stack and Debugging

### Call Stack

- Is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions. 

- The call stack is synchronous.

- A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation.

### Flow of a Call Stack

- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.

- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.

- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.

- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

## Errors

- Reference errors - when you try to use a variable that is not yet declared you get this type of errors.

- Syntax errors - this occurs when you have something that cannot be parsed in terms of syntax.

- Range errors - try to manipulate an object with some kind of length and give it an invalid length.

- Type errors -  when the types you are trying to use or access are incompatible.

### Debugging

 - The easiest and maybe the most common way its to simply `console.log()` the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).