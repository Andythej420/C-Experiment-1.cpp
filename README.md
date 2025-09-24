# C-Experiment-1.cpp

# Experiment 1: Hello World & Basic Calculator

## Aim
- Write a C++ program to print "Hello, World!"  
- Build a simple calculator to perform addition, subtraction, multiplication, and division  

---

## Objectives
- Understand the structure and flow of a basic C++ program  
- Learn to use cout for output and cin for user input  
- Understand the purpose of using namespace std;  
- Use // to write meaningful comments for better code clarity  

---

## Program Explanation
- `#include <iostream>` : Adds input-output functionality  
- `using namespace std;` : Lets us use standard library features like cout and cin without prefixing `std::`  
- `int main()` : Entry point of every C++ program  
- `return 0;` : Indicates successful program execution  
- `cout` : Prints output to the console  
- `cin` : Takes input from the user  
- `//` : Used for single-line comments  
- Arithmetic Operators: `+`, `-`, `*`, `/` are used for calculations  
- `float` : Stores decimal number inputs  
- Every statement ends with a semicolon (;)  

---

## C++ Code

```cpp
// Experiment 1: Hello World & Basic Calculator
#include <iostream>
using namespace std;

int main() {
    // Part 1: Hello World
    cout << "Hello World" << endl;

    // Part 2: Basic Calculator
    float num1, num2;

    // Taking input from the user
    cout << "Enter num1: ";
    cin >> num1;
    cout << "Enter num2: ";
    cin >> num2;

    // Performing operations
    cout << "Sum: " << num1 + num2 << endl;
    cout << "Difference: " << num1 - num2 << endl;
    cout << "Product: " << num1 * num2 << endl;

    // Division (check for divide by zero)
    if (num2 != 0) {
        cout << "Division: " << num1 / num2 << endl;
    } else {
        cout << "Division: Undefined (cannot divide by zero)" << endl;
    }

    return 0;
}
