# Hello World

All this information might be overwhelming, so let's write our first real `C++` program. 

The source code of the following two programs can be found in `./code/`. They demonstrate the basic syntax or anatomy of a `C++` program and most programming tutorials, books or the like start with such a `hello world` program. The code does nothing but print the `string` (a bunch of characters) to the screen (or `standard output`, abbreviated as `stdout`; [click here](https://en.wikipedia.org/wiki/Standard_streams#Standard_output_(stdout)) for more information regarding this terminology).

```c++
#include <iostream>

using namespace std;

int main() {
    cout << "hello world" << endl;
    return 0;
}
```




[previous](./basic_syntax.md) | [next]()
