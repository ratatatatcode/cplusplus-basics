Let’s say you want a program that prints the numbers from 1 to 1000 and tells whether each number is even or odd, but you’re just as lazy as I am. You wouldn’t write code like this:
```cpp
#include <iostream>
using namespace std;

int main()
{
    cout << "1 is an odd number." << endl;
    cout << "2 is an even number." << endl;
    cout << "3 is an odd number." << endl;
    cout << "4 is an even number." << endl;
    cout << "5 is an odd number." << endl;
    cout << "6 is an even number." << endl;
    cout << "7 is an odd number." << endl;
    cout << "8 is an even number." << endl;

    return 0;
}
```

Here's how the **loop** comes in handy. I will show you an example and try to run this code by yourself.
```cpp
#include <iostream>
using namespace std;

int main()
{
    for (int i = 1; i <= 100; i++) {
        if (i % 2 == 0) cout << i << " is an even number" << endl;
        else cout << i << " is an odd number" << endl;
    }

    return 0;
}
```

```cpp
#include <iostream>
using namespace std;

int main()
{
    for (int i = 1; i <= 100; i++)
        // Ternary Operator
        cout << i << (i % 2 == 0 ? " is an even number" : " is an odd number") << endl;

    return 0;
}
```