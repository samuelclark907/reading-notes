# Read-03: FileIO & Exceptions

## What is a file?

- Most modern file systems are made up of three parts:

1. Header - Metadata about the contents of the file.

2. Data - Contents of the file as written by the creator or editor.

3. End of file (EOF) - Special character that indicates the end of the file.

### File paths

- The file path is a string that represents the location of a file. Three mayjor parts.

1. Folder Path - the file folder location on the file system where subsequent folders are separated by a forward slash.

2. File Name -  the actual name of the file.

3. Extension - the end of the file path pre-pended with a period (.) used to indicate the file type.

### Examples to open files

- `open('abc.txt')`

- `open('abc.txt', 'r')`

- `open('abc.txt', 'w')`

### Reading and Writing Opened Files

`.read(size=-1)` - This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.

`.readline(size=-1)` - This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.

`.readlines()` - This reads the remaining lines from the file object and returns them as a list.

### Built in libraries.

`wave:` read and write WAV files (audio)

`aifc:` read and write AIFF and AIFC files (audio)

`sunau:` read and write Sun AU files

`tarfile:` read and write tar archive files

`zipfile:` work with ZIP archives

`configparser:` easily create and parse configuration files

`xml.etree.ElementTree:` create or read XML based files

`msilib:` read and write Microsoft Installer files

`plistlib:` generate and parse Mac OS X .plist files

### Raising an Exception

- We can use `raise` to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

### The AssertionError Exception

- Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met.

### Summary

- `raise` allows you to throw an exception at any time.

- `assert` enables you to verify if a certain condition is met and throw an exception if it isn’t.

- In the `try` clause, all statements are executed until an exception is encountered.

- `except` is used to catch and handle the exception(s) that are encountered in the try clause.

- `else` lets you code sections that should run only when no exceptions are encountered in the try clause.

- `finally` enables you to execute sections of code that should always run, with or without any previously encountered exceptions.