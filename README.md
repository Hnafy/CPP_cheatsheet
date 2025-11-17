# C++ Reference Guide

*Created by Ahmed Naser :)*

---

## Table of Contents
1. [Basic Data Types](#basic-data-types)
2. [Conditions](#conditions)
3. [Loops](#loops)
4. [Math Functions](#math-functions)
5. [String Functions](#string-functions)
6. [Arrays](#arrays)
7. [User Input](#user-input)
8. [User-Defined Functions](#user-defined-functions)
9. [Tips & Tricks](#tips--tricks)

---

## Basic Data Types

C++ provides several fundamental data types:

- **int** - Integer numbers
- **float** - Floating-point numbers (can have up to 7 digits after decimal point)
- **double** - Double-precision floating-point (can have up to 15 digits after decimal point)
- **bool** - Boolean values (true/false)
- **char** - Single characters

---

## Conditions

### If-Else Statement

```cpp
int z = 10;
if (z == 5) {
  cout << "it is 5" << endl;
} else if (z == 10) {
  cout << "it is 10";
} else {
  cout << "none of them";
}
```

**Note:** Use `==` for comparison, not `=` (which is assignment).

### Switch Statement

Switch statements accept variables, while cases accept specific values:

```cpp
switch (z) {
case 10:
  cout << "go on";
  break;
default:
  cout << "it is default output in switch" << endl;
  break;
}
```

---

## Loops

### For Loop

For loops accept conditions and variables:

```cpp
for (int i = 0; i <= 3; i++) {
  cout << i << endl;
}
```

### While Loop

While loops accept conditions:

```cpp
int i = 0;
while (i <= 3) {
  cout << i << endl;
  i++;
}
```

### Do-While Loop

Do-while loops execute code first, then enter the loop:

```cpp
int y = 0;
do {
  cout << y << endl;
  y++;
} while (y <= 3);
```

---

## Math Functions

**Required:** `#include <cmath>`

```cpp
float a = 2.7;
int x = 2;
int p = 4;

// Rounding functions
cout << "floor 2.7 = " << floor(a) << endl;  // Round down to nearest integer
cout << "ceil 2.7 = " << ceil(a) << endl;    // Round up to nearest integer
cout << "rint 2.7 = " << rint(a) << endl;    // Round to nearest integer (returns double)

// Comparison functions
cout << "fmax(2, 4) = " << fmax(x, p) << endl;  // Return larger of x and p
cout << "fmin(2, 4) = " << fmin(x, p) << endl;  // Return smaller of x and p

// Arithmetic functions
cout << "fmod(2, 4) = " << fmod(x, p) << endl;  // Floating-point remainder of x/p
cout << "pow(2, 4) = " << pow(x, p) << endl;    // Raise x to the power p
cout << "sqrt(4) = " << sqrt(p) << endl;        // Square root of p
cout << "cbrt(8) = " << cbrt(8) << endl;        // Cube root of 8
```

---

## String Functions

```cpp
string s = "ahmed";

cout << s.length() << endl;              // Returns number of characters in string
cout << s.substr(0, 3) << endl;          // Returns substring starting at index 0 with length 3
cout << s.find("h") << endl;             // Finds position of first occurrence of "h"
cout << s.append(" naser") << endl;      // Adds text to the end of the string
cout << s.replace(0, 5, "saif") << endl; // Replaces 5 chars from index 0 with "saif"
cout << s.empty() << endl;               // Returns true if string is empty, false otherwise
```

---

## Arrays

### Traditional For Loop

```cpp
string fruits[] = {"Apple", "Banana", "Orange"};
int n = size(fruits);

for (int i = 0; i < n; i++) {
  cout << fruits[i] << endl;
}
```

### Range-Based For Loop

```cpp
for (string element : fruits) {
  cout << element << endl;
}
```

---

## User Input

To handle user input with spaces, use `getline()`:

```cpp
string name;
cout << "Enter your name: ";
getline(cin, name);  // Reads entire input line (including spaces) before Enter is pressed
cout << "Welcome " << name;
```

---

## User-Defined Functions

Functions can have default parameter values:

```cpp
void greeting(string name = "default name") {
  cout << "welcome " << name << endl;
}
```

**Function Types:**
- Functions can return any C++ data type (int, double, bool, string, etc.)
- If a function does not return any value, use `void` instead of a return type

---

## Tips & Tricks

### Variable Operations

- **Declaration** - Defining a variable without giving it a value
- **Assigning** - Giving a value to a variable that has already been created
- **Initialization** - Defining a variable and giving it a value directly when it is created

### Ternary Operator

```cpp
int b = condition ? value_if_true : value_if_false;
```

### Function Types

- **Built-in Functions** - Functions already provided by C++
- **User-defined Functions** - Functions created by the programmer

### Important Notes

- Always use `==` for comparison in conditions, not `=`
- Use `break` statements in switch cases to prevent fall-through
- Remember to include necessary headers (`<cmath>` for math functions, `<iostream>` for I/O)
