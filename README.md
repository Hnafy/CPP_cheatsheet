# C++ Cheat Sheet

Use this sheet to quickly recall the most important C++ foundations before diving into competitive programming!

---

## **Basic Data Types — The Building Blocks**\*\*

-   `int` – Integer numbers
-   `float` – Decimal numbers (≈ 7 digits precision)
-   `double` – Decimal numbers (≈ 15 digits precision)
-   `bool` – true / false
-   `char` – Single character

---

## **Conditions — Control the Flow**\*\*

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

### `switch` Statement

```cpp
switch (z) {
case 10:
    cout << "go on";
    break;
default:
    cout << "default case" << endl;
    break;
}
```

---

## **Loops — Repeat Smartly**\*\*

### `for`

```cpp
for (int i = 0; i <= 3; i++) {
    cout << i << endl;
}
```

### `while`

```cpp
int i = 0;
while (i <= 3) {
    cout << i << endl;
    i++;
}
```

### `do while`

```cpp
do {
    cout << y << endl;
    y++;
} while (y <= 3);
```

---

## **Math Functions — For Fast Calculations**\*\* _(requires ********\*\*\*\*********#include \<cmath>********\*\*\*\*********)_

```cpp
float a = 2.7;
int x = 2;
int p = 4;

floor(a);   // round down
o ceil(a);    // round up
o rint(a);    // round to nearest integer (double)

fmax(x,p);  // max value
fmin(x,p);  // min value
fmod(x,p);  // remainder of x / p

pow(x,p);   // x^p
sqrt(p);    // square root
cbrt(8);    // cube root
```

---

## **String Functions — Text Handling Essentials**\*\*

```cpp
string s = "ahmed";

s.length();        // number of characters
s.substr(0, 3);    // substring from index 0 length 3
s.find("h");       // find index of 'h'
s.append(" naser");
s.replace(0,5,"saif");
s.empty();         // true if string is empty
```

---

## **Arrays — Store Multiple Values**\*\*

```cpp
string fruits[] = {"Apple", "Banana", "Orange"};
int n = size(fruits);

for (int i = 0; i < n; i++) {
    cout << fruits[i] << endl;
}

for (string element : fruits) {
    cout << element << endl;
}
```

---

## **Input — Read User Data**\*\*

```cpp
string name;
cout << "Enter your name: ";
getline(cin, name);
cout << "Welcome " << name;
```

---

## **Functions — Reusable Code Blocks**\*\*

```cpp
void greeting(string name = "default name") {
    cout << "welcome " << name << endl;
}
```

---

## 💡 **Tips & Tricks — Write Cleaner & Faster Code**\*\*

-   Declaring a variable without value → **Declaration**
-   Giving an existing variable a value → **Assigning**
-   Declaring + assigning in one step → **Initialization**

### **Ternary Operator**

```cpp
int b = condition ? value_if_true : value_if_false;
```

### **Types of Functions**

-   Built‑in functions → provided by C++
-   User‑defined functions → created by programmer

If a function returns nothing, use **void**.

---

### ✍️ **Created by:** Ahmed Naser
