# READ-CLASS-09

## Dunder Methods

### What are Dunder Methods

- They are easy to recognize because they start and end with double underscores.

- Dunder methods let you emulate the behavior of built-in types.

### Special Methods and the Python Data Model

- You can see Python’s data model as a powerful API you can interface with by implementing one or more dunder methods.

- To construct account objects from the Account class I need a constructor which in Python is the `__init__` dunder.

- `__repr__`: The “official” string representation of an object. This is how you would make an object of the class. The goal of __repr__ is to be unambiguous.

- `__str__`: The “informal” or nicely printable string representation of an object. This is for the enduser.

- `__len__` and `__getitem__` are used to iterate over a non iterable item and getitem retrieves the value.

- You can make an object callable like a regular function by adding the `__call__` dunder method.

## Statistics Probablity

### What is probability?

- At the most basic level, probability seeks to answer the question, “What is the chance of an event happening?” An event is some outcome of interest.

### The Data and Distribution

- The normal distribution refers to a particularly important phenomenon in the realm of probability and statistics.

- We started with descriptive statistics and then connected them to probability. From probability, we developed a way to quantatively show if two groups come from the same distribution.