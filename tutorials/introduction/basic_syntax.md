# Basic C++ Syntax

The basic syntax of `C++` is fairly simple and only consists of a few core elements. They will be demonstrated in the this section. The following list is meant to provide an overview of the building blocks of `C++`. It is not meant to be an exhaustive collection of all `C++` language features. All concepts will be explained in greater detail along the way and we will add to this list in later chapters, too.

Before we start, note the following:

```c++
// in C++, two forward slashes denote a single line comment
/* a multi-line comment can be created using a forward slash
and a star at the start and at the end of the comment */
```

While all code examples have a certain color scheme to make them easier to read, your IDE or text editor might do syntax highlighting slightly differently. Do not get confused! The color is never part of the code itself (code or programs are just text instructions) and is only there to help us identify certain patterns like which lines are comments or pre-processor instructions (a topic that will be discussed shortly). Now, let's look at common syntax elements of `C++` (and really, almost all modern programming languages):


## Variables

Variables hold data for re-use ...

## Statements

A statement is a unit of code that is terminated by a semicolon `;`. There are multiple ways in which statements are used in C++, for example

```c++
// to declare variables
int x;

// to initialize variables
int x = 5;

// to assign values to variables that were previously declared
int x;
x = 5;

// to call functions, for example `printf()'
printf("5 + 8 = %d\n", 5+8);
```

## Expressions



## Functions

A function is a larger unit of code that itself contains statements. The most prominent function is `main()` because it is the main entry point of a C++ program, no matter if it is a command line program, a web application or an operation system.

```c++
// function `main' is the entry point for your C++ application
int main(int argc, char **argv) {
    cout << "Hello World" << endl;
    return 0;
}
```

## Classes






[previous](./setup.md) | [next](./hello_world.md)
