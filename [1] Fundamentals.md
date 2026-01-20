```c++
#include <iostream>

int main()
{
    std::cout<<"Hello World";

    return 0;
}
```

```c++
#include <iostream>
```
This is a **header file library**. It allows you to input (cin) and output (cout) objects.

As you can see, I used std:: before cout. This means that it comes from the C++ standard library.

You can avoid writing them as the code gets longer by using **using namespace std**.

```c++
#include <iostream>
using namespace std;

int main()
{
    cout<<"Hello World";

    return 0;
}
```

Let's move on to **int main() { }**. Every statement or code inside it will be executed.

**cout** is used to display text or output on the screen.

**return 0** isn’t strictly necessary in modern C++, as the program works the same without it. Older versions of C++ required it. The 0 tells the operating system that the program finished successfully.

**What else should I know before moving on to more advanced C++ topics?**

**Identifiers** are the unique names for your classes, functions, objects, variables, or other entities in your program.
```c++
int age = 22
void add() {}
```

**Keywords** are predefined, reserved keywords that have special meanings to the compiler and can't be used as identifiers.
```c++
int
return
```

**Variable** is a name for a memory location. The value stored in a variable can be referenced and changed during the execution.
```c++
int main()
{
    int age = 22;
    age = 23;

    cout << age;

    return 0;
}
```

**Data Types**
**Basic Data Types**<br>
- int (1, 2, 3, 4, 5, 6)
- float (3.14 - values in the range from 1.2e-38 to 3.4e+38)
- double (3.14159... - values in the range from 1.7e-308 to 1.7e+308)
- char ('A' 'a' 'B' 'b' 'C' 'c')
- bool (true, false)
- void

**Derived Data Types**
- array
- pointer
- reference
- function

**User Defined Data Types**
- class
- structure
- union
- typedef
- using