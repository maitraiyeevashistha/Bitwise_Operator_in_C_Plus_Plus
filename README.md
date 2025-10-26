#  Bitwise Operators in C++

## Title: Understanding and using Bitwise Operators in C++
---
## Aim :
*To study and implement C++ Bitwise Operators.*

##  Introduction

Bitwise operators in C++ are used to perform operations directly on the **bits** of an integer. Bitwise operators perform operations on the binary representations of integers. Unlike arithmetic or logical operators that act on whole values, bitwise operators let you manipulate data at the binary level . The 1s and 0s that computers actually work with. They are useful for low-level programming tasks, such as manipulating data at the bit level or optimizing performance in critical sections of code.

##  Types of Bitwise Operators

Each operator works **bit-by-bit** on the integers.

### 1. AND (`&`) — Bitwise AND

Performs a logical `AND` between corresponding bits of two numbers. Resulting bit is 1 only if both input bits are 1. (Returns 1 **only** if both corresponding bits are 1.)

### 2. OR (`|`):
Performs a logical OR. Resulting bit is 1 if at least one of the input bits is 1.Compares each bit of two operands; the result has a bit set to 1 if either of the corresponding bits of the operands is 1

### 3. XOR (`^`):
Performs a logical exclusive OR. Resulting bit is 1 only if the input bits are different.Compares each bit of two operands; the result has a bit set to 1 if only one of the corresponding bits of the operands is 1, but not both.

### 4. NOT (`~`):
Unary operator that inverts (flips) all bits of a number.(Inverts all the bits of the operand. Each 0 becomes 1 and each 1 becomes 0.)

### 5. Left Shift (`<<`):
Shifts all bits to the left by a specified number of positions, inserting 0s on the right. Equivalent to multiplying by powers of 2.

### 6. Right Shift (`>>`):
Shifts all bits to the right. Useful for dividing integers by powers of 2.

## Summary of the programs 

### Program 1 : Bitwise Operator 

This program demonstrates how the bitwise AND, OR, NOT, XOR, left shift, and right shift work on two integers.

 - `AND` returns 1 only if both bits are 1.
 - `OR` returns 1 if at least one bit is 1.
 - `XOR` returns 1 if the bits are different.
 - `NOT` flips each bit (used for one's complement).
 - `Left` Shift multiplies a number by 2ⁿ.
 - `Right` Shift divides a number by 2ⁿ.
 
### Sample Output:
Enter the bit position to be set: 5               
Enter the bit position to be reset: 3               
Your number is:56            
Your number is:16                
##  Program 2: Set and Reset Specific Bits

This program illustrates how to **set/change individual bits** of an integer using bitwise operations. 

###  Setting a Bit
To **set** a bit in a number, we use the **bitwise OR (`|`)** operator with a **bitmask**.  
A bitmask is a binary number where only the target bit is `1` and all others are `0`.
To reset a bit we use **bitwise AND (`&`)** with the complement (~) of a mask where the target bit is 1.

### Sample Output:
AND: 0               
OR:6                  
NOT: -5              
XOR: 6                 
right shift: 1                
left shift: 4               

## Conclusion 
Bitwise operators let you work directly with the individual bits of data. They’re useful when you need to control things very precisely, like when dealing with hardware or saving memory. The programs above show how to use these operators for simple tasks like turning specific bits on or off, or combining bits using logic.






