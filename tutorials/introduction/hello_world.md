# Hello World

## Introduction

All this information might be overwhelming, so let's write our first real `C++` program. 

The source code of the following two programs can be found in `./code/`. They demonstrate the basic syntax or anatomy of a `C++` program and most programming tutorials, books or the like start with such a `hello world` program. The code does nothing but print the `string` (a bunch of characters) to the screen (or `standard output`, abbreviated as `stdout`; [click here](https://en.wikipedia.org/wiki/Standard_streams#Standard_output_(stdout)) for more information regarding this terminology).

*./code/hello_world_00.cpp*

```c++
#include <iostream> // pre-processor instruction

using namespace std; // namespaces


/* the main loop starts here */
int main() {
    cout << "hello world" << endl; // output a string to the screen
    return 0; // return statement
}
```

When compiled and run from the command line, this program prints `hello world` to the screen. As we've seen before, the human-readable version of the program must be translated into a machine-readable form before the CPU can successfully follow our instructions. It is a nice feature of `C++` and most modern high-level computer languages, that we do not have to think in machine code (or [assembler](https://en.wikipedia.org/wiki/Assembly_language)) but in a language that is closer to the language we speak every day.

Similar to natural languages, computer languages are composed of `tokens`. Tokens can be classified into sub-groups (comparable to verbs, nouns, adjectives, ...) and they are separated from each other by white spaces or new-line characters. That means that we could have written our program in the following form:

```c++
// ...

int 
main
()
{
cout

// ...

```

But that is not very legible so tokens that form logical units (like `int main()`) are usually grouped together.

Now, let's take a look at the tokens (or words) that we used in the `hello world` program.


## Pre-processor instructions

The first few tokens (that are not comments, i.e. not `// ...` or `/* ... */`) are so-called [pre-processor](https://en.wikipedia.org/wiki/C_preprocessor) instructions. They start with a `#` sign and they are not part of `C++` itself. The pre-processor will be covered in greater detail later, but generally speaking, it provides the ability to include information from other files (library files that describe helpful functions for example) in your program. In the program above, the pre-processor (which is invoked by the compiler in an initial step before actual compilation) is instructed to literally **include** a header file which provides functions for input and output (thus *IO*) of e.g. characters or strings to and from the screen.

If you try to run the program without this instruction, the compiler will not be able to interpret the `cout` token.


## Namespaces

Again, namespaces will be discussed in greater detail soon. Suffice to say that `using namespace std;` allows us to omit the source of functions, objects, etc. when we use them in our code. Without this line, we would have to write for example `std::cout` to let the compiler know that `cout` is defined in the standard library (i.e. a different namespace). At this point, just remember to include this somewhat magical line of code to simplify the process of calling upon things that are defined in libraries that we are just using but did not write ourselves.


## Main Loop



[previous](./basic_syntax.md) | [next]()
