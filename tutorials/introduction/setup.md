# Setup a Programming Environment

## Overview

`C++` is a compiled programming language. That means, a so-called `compiler` is required to convert `C++` source code into runnable programs. Many different `C++` exist and they reflect the evolution of the language itself, i.e. not all compilers support the latest `C++` standards or implement them in different ways. Bjarne Stroustrup list a variety of common compilers on his [website](http://www.stroustrup.com/compilers.html), though. The major compiler vendors all support the latest `C++` language features and many of them are available for free and/or open-sourced. To follow along, it is recommended that you install an up-to-date `C++` compiler and a text editor that supports syntax highlighting for `C++`. The latter is not striktly required, though (instead, you could write `C++` source code using the terminal-based editor [Vim]() that is pre-installed on all Unix-based operating systems or [Notepad]() on Windows). 

Examples of such editors are [Sublime Text](https://www.sublimetext.com/) and [Atom](https://atom.io/). They are often called IDEs (Integrated Development environments), because they provide many more features in addition to syntax highlighting, e.g. linting (tools that flag potential stylistic or syntax errors on the fly) and code completion. Search the internet for more information on how to set up an IDE for writing `C++` programs!

## What Does a Compiler Do?

There are two fundamentally different types of programming languages, interpreted (or scripting) languages like `Python` ... and compiled languages like `C`/`C++` or `Go`.

## Compile a C++ Program

If you happen to have a computer that runs Windows as an operating system, I highly recommend to look at this [tutorial](https://msdn.microsoft.com/en-us/library/ms235639.aspx) by Microsoft. It explains the setup step-by-step and after completing it, you will be able to compile and run `C++` programs.

In a Linux or Mac environment, the process is slightly easier. You can either use the [GCC]() or [Clang]() compiler, both are usually pre-installed. To test your setup, download the file `hello_world.cpp` from the `code/` directory of this repository. Next, open a terminal window and navigate to the folder into which you saved `hello_world.cpp`. Either one of the following commands will compile the source code in `hello_world.cpp` into an executable file called `hello_world` (note: without any file extension on Mac/Linux, executables under Windows have the extension `.exe`):

```bash
# to compile a C++11 (2011 standard) program with GCC
g++ -std=c++11 hello_world.cpp -o hello_world 

# to compile a C++11 program with Clang
clang++ -std=c++11 -stdlib=libc++ hello_world.cpp -o hello_world

# to run the newly created executable
./hello_world
```

The programs that contain the compilers are called `g++` and `clang++`. They need additional instructions to correctly compile `C++` source code and these instructions are provided as so-called command-line flags. Flags are just additional arguments and they are usually specified according to the schema `-<argument_name>`. `std=c++11` tells the compiler to use features that were introduced in `C++` standard 11. Clang needs an additional flag to function properly, `-stdlib=libc++`. This argument tells Clang to use the `C++` standard library. In both compiler instructions, the name of the source code file follows next. Lastly, the `-o` flag specifies the name of the output executable (in this example `hello_world`).


[previous](./introduction.md) | [next](./basic_syntax.md)
