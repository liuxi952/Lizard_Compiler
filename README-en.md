# Lizard Compiler

Lizard Compiler is a lightweight C++-based scripting interpreter project designed to demonstrate the fundamental structure of an interpreter, including lexical analysis, expression parsing, bytecode generation, and virtual machine execution.

This project started as a teaching-oriented internal preview version. It already supports basic script execution and is suitable for learning interpreter principles, virtual machine design, and the basic workflow of compiling and running a simple language.

## Features

- Supports print statements
- Supports variable definition and assignment
- Supports basic arithmetic expressions: +, -, *, /
- Supports comparison expressions: >, <, >=, <=, ==, !=
- Supports string literals
- Supports if / else branches
- Supports while loops
- Supports ++ and -- increment/decrement operations
- Supports return statements
- Supports running scripts from .cl files

## Example Code

```cl
int i = 0
while(i < 2) {
    i++
}
print i
```

Another simple example:

```cl
int a = 3
int b = 5
print a + b
print "Hello, Lizard!"
```

## Project Structure

- Lizard/Lizard/Lizard.cpp: main program, lexical analysis, syntax compilation, and virtual machine execution logic
- Lizard/test.cl: example script file

## How to Run

1. You can run the executable directly in the folder and pass in a .cl script file:

```bash
Lizard.exe test.cl
```

If you want to register .cl file association, you can also run:

```bash
Lizard.exe --register
```

## Notes

The current version is still a lightweight interpreter focused on demonstrating core implementation ideas. It can be extended in the future to support a more complete scripting language, such as:

- Function definitions and calls
- More data types
- More robust syntax error handling
- Richer control flow support
