**Operators**

**1. Arithmetic Operators**
- [+] Addition (num_a + num_a)
- [-] Subtraction (num_a - num_b)
- [*] Multiplication (num_a * num_b)
- [/] Division (num_a / num_b)
- [%] Modulo Operation (num_a % 2)
- [++] Increment (pre-increment: ++num, post-increment: num++)
- [--] Decrement (pre-decrement: --num, post-decrement: num--)
```cpp
#include <iostream>
using namespace std;

int main()
{
    int num_a = 4, num_b = 2;
    cout << num_a + num_b << endl; // Output: 6
    cout << num_a - num_b << endl; // Output: 2
    cout << num_a * num_b << endl; // Output: 8
    cout << num_a / num_b << endl; // Output: 2
    cout << num_a % num_b << endl; // Output: 0

    num_a++;
    cout << num_a << endl; // Output: 5
    num_b--;
    cout << num_b << endl; // Output: 1

    // Tricky Part of Increment: pre-increment affects the condition, post-increment doesn’t (yet)
    int test_a = 5;
    if (++test_a == 6) cout << "True"; // test_a value: 6
    cout << endl;
    int test_b = 5;
    if (test_b++ == 6) cout << "True"; // test_b value: 5
    else cout << "False";

    return 0;
}
```

**2. Relational Operators**<br>
- [==] Is Equal To
- [\>] Greater Than
- [\>=] Greater Than or Equal To
- [<] Less Than
- [<=] Less Than or Equal To
- [!=] Not Equal To
```cpp
#include <iostream>
using namespace std;

int main()
{
    int num_a = 1, num_b = 2;
    // cout will print either 0 (false) or 1 (true).
    cout << (num_a == num_b) << endl; // Output: 0
    cout << (num_a > num_b) << endl; // Output: 0
    cout << (num_a >= num_b) << endl; // Output: 0
    cout << (num_a < num_b) << endl; // Output: 1
    cout << (num_a <= num_b) << endl; // Output: 1
    cout << (num_a != num_b) << endl; // Output: 1

    return 0;
}
```

**3. Logical Operators**<br>
- [&&] Logical AND (true && true)
- [||] Logical OR (true || false - at least one is true)
- [!] Logical NOT ()
```cpp
#include <iostream>
using namespace std;

int main()
{
    bool bool_a = true, bool_b = false;
    // cout will print either 0 (false) or 1 (true).
    cout << (bool_a && bool_b) << endl; // Output: 0
    cout << (bool_a || bool_b) << endl; // Output: 1
    cout << (!bool_a) << endl; // Output: 0

    return 0;
}
```

**4. Bitwise Operators**<br>
- [&] Binary AND 
- [|] Binary OR 
- [^] Binary XOR 
- [<<] Left Shift 
- [\>\>] Right Shift 
- [~] One's Complement 

**5. Assignment Operators**<br>
- [=] Assignment
- [+=] Add and Assignment
- [-=] Subtract and Assignment
- [*=] Multiply and Assignment
- [/=] Divide and Assignment

**6. Ternary or Conditional Operators**
- Expression1 ? Expression2: Expression3