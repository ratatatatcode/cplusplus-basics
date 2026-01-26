Since we already know how logical and relational operators work. We can now proceed with **conditional statement (if-else if-else)**.

Common interview question is **Fizz buzz**:<br>
Input an integer and determine whether it should be printed as "Fizz", "Buzz", "FizzBuzz", or the number itself.
- If a number is divisible by 3, print "Fizz"
- If a number is divisible by 5, print "Buzz"
- If a number is divisible by both 3 and 5, print "FizzBuzz"
- Otherwise, print the number itself

**What is my thought process?**
First, I will check if the number is divisible by both 3 and 5. If this check is done later, numbers like 15 and 30 would print "Fizz" or "Buzz" instead of "FizzBuzz".

Next, I will use else if. When the condition in the if statement (FizzBuzz) is false, the code inside the else if block will be executed. In these conditions, we check whether the number is divisible by 3 or 5.

Should we include printing the number itself in an else if statement? Definitely not. Doing so would require many unnecessary conditions. For example, if the number is 4, it would pass the first three checks, and since it is divisible by 2, we might incorrectly print 2 or other values.

Instead, by using a final else statement, any number that does not meet the first three conditions will simply print the number itself.

> “I first check divisibility by both 3 and 5 to handle FizzBuzz correctly. Then I check divisibility by 3 or 5 individually. If none of the conditions match, I print the number itself.”

```cpp
#include <iostream>
using namespace std;

int main()
{
    int num;
    cout << "Number: ";
    cin >> num;
    
    if (num % 3 == 0 && num % 5 == 0) cout << "FizzBuzz";
    else if (num % 3 == 0) cout << "Fizz";
    else if (num % 5 == 0) cout << "Buzz";
    else cout << num;

    return 0;
}
```