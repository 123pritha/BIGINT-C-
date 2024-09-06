# BIGINT c++
<p>
This function is used to make operations with c++ easier using big integers and it performs operations such as adding,subtracting , multiplication,square root, factorial, fibonacci series etc on big integers.
Since C++ does not have a built-in BigInt type, such functionality can be achieved by creating a custom class or by using third-party libraries like GMP (GNU Multiple Precision Arithmetic Library) or Boost.Multiprecision.
# BigInt Implementation in C++

This project is a custom implementation of a **BigInt** class in C++ to handle integers larger than the standard data types (like `int` or `long long`). The **BigInt** class supports basic arithmetic operations such as addition, subtraction, multiplication, and division for arbitrarily large integers.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Examples](#examples)

## Features

- Supports large integer operations (beyond 64-bit integers).
- Basic arithmetic operations:
  - Addition
  - Subtraction
  - Multiplication
  - Division
  - Modulo
- Comparison operators (`==`, `!=`, `<`, `<=`, `>`, `>=`).
- Input/Output operations using the `<<` and `>>` stream operators.
- Handles negative numbers.

## Technologies Used

- **C++ (C++11 and above)** for the implementation.
- Standard C++ libraries such as:
  - `<iostream>` for input/output operations.
  - `<string>` for handling large numbers as strings.
  - `<vector>` and `<algorithm>` for internal data structures.

## usage
[Examples](#examples)

#include "bigint.h"

int main() {
    BigInt num1("12345678901234567890");
    BigInt num2("98765432109876543210");
    BigInt result = num1 + num2;
    std::cout << "Sum: " << result << std::endl;
    
}
BigInt a("12345678901234567890");
BigInt b("98765432109876543210");
BigInt sum = a + b;
std::cout << "Sum: " << sum << std::endl;
// Output: Sum: 111111111011111111100



BigInt a("98765432109876543210");
BigInt b("12345678901234567890");
BigInt diff = a - b;
std::cout << "Difference: " << diff << std::endl;
// Output: Difference: 86419753208641975320



BigInt a("12345678901234567890");
BigInt b("98765432109876543210");
BigInt product = a * b;
std::cout << "Product: " << product << std::endl;
// Output: Product: 1219326311370217952237463801111263526900



BigInt a("12345678901234567890");
BigInt b("98765432109876543210");

if (a < b) {
    std::cout << "a is smaller than b" << std::endl;
} else {
    std::cout << "a is not smaller than b" << std::endl;
}
// Output: a is smaller than b



</p>
