# Chapter 1 Notes Simplified
## Table of Contents
- [Number Representations](#Number-Representations)
	- [Binary Representation](#Binary-Representation)
- [Decimal Binary Conversion](#Decimal-Binary-Conversion)
	- [Subtraction Method](#Subtraction-Method)
	- [Addition Method](#Addition-Method)
	- [Division Method](#Division-Method)
- [Binary Arithmetic](#Binary-Arithmetic)
	- [Binary Addition](#Binary-Addition)
	- [Binary Subtraction](#Binary-Subtraction)
	- [Binary Multiplication](#Binary-Multiplication)
- [Bytes](#Bytes)
- [Hexadecimal Representation](#Hexadecimal-Representation)
	- [Decimal Conversion to Hexadecimal](#Decimal-Conversion-to-Hexadecimal)
	- [Hexadecimal Conversion to Decimal](#Hexadecimal-Conversion-to-Decimal)
	- [Binary Conversion to Hexadecimal](#Binary-Conversion-to-Hexadecimal)
- [Octal System](#Octal-System)
- [Representing Negative Numbers](#Representing-Negative-Numbers)
# Number Representations
**Binary (Base 2 Number System)** - 1s and 0s <br />
**Base 10 (Decimal / *positive* counting numbers)** - 1, 2, 3 and so on
<br />
### Equation for Base 10 Numbers
![](Photos/Base%2010%20Equation.png) <br />
![](Photos/Example%20simplified.png) <br />
#### Theorem 1: 
![](Photos/Theorem%201.png) <br />
![](Photos/Theorem%201%20Example.png) <br />
![](Photos/Theorem%201%20Example%20Colorized.png) <br />
**b (3)** will always be the sub number next to the **integer (a = 201)**.
In order to get the exponents for **b**, set **b = k**, and you subtract 1 from **k**, **k - 1**.
## Binary Representation
Base = 2 <br />
0 < Integers (a<sub>k</sub>) < 2 <br />
![](Photos/Binary%20Representation%20Example.png) <br />
This is the same case as theorem 1, but this time in binary.
# Decimal-Binary Conversion
## Subtraction Method
![](Photos/Subtraction%20Method.png) <br />
## Addition Method
![](Photos/Addition%20Method.png) <br />
You only add the values of the 1s and not the 0s to figure out the decimal value.
In this case: 32 + 16 + 4 + 2 = 54
## Division Method
1) You are dividing each number by 2 plus a remainder
2) If the number is a whole number *(ex: 1, 4, 6)* then the remainder will be 0. If the number is not a whole number *(ex: 1.75, 1.25)* then the remainder will be 1. If the number is not a whole number, round up to the nearest whole number *(ex: 1.75 -> 2)*.
3) In order to get the binary result, start from the very bottom and work your way up. It'll be like this -> left most side (started from the bottom number) to the right most side (the top number).
![](Photos/Division%20Method.png)
# Binary Arithmetic
## Binary Addition
![](Photos/Binary%20Addition%20Rules.png)
<br />
![](Photos/Binary%20Addition%20Example.png)
<br />
Should be really easy to understand
## Binary Subtraction
![](Photos/Binary%20Subtraction%20Rules.png) <br />
![](Photos/Binary%20Subtraction%20Example.png)  <br />
## Binary Multiplication
![](Photos/Binary%20Multiplication.png) <br />
It should just be like regular multiplication.
# Bytes
**Byte** - An 8 bit binary number with leading zeros allowed. There are 256 different types of bytes ranging from 0 (00000000) to 255 (11111111). <br />
**Word** - A basic unit of storage that depends on the size of a particular computer. Words tend to be composed of 4 **(32 bit)** or 8 **(64 bit)** bytes. <br />
**ASCII** - Uses the lower 7 bits of a byte, 0 - 127, to represent letters and special characters like [these](https://www.geeksforgeeks.org/ascii-table/) <br />
**ISO Latin-1 and Mac-Roman (Obsolete)** - Uses values above 127 for accented letters as well as addition special characters. <br />
**Unicode (UTF-32 / USC-4)** - AN international standard intended to encode all characters in all languages as well as mathematical and other specialized characters. They use 4 bytes to encode unicode characters. <br />
# Hexadecimal Representation
**Hexadecimal** - Uses regular decimal digits as well as A, B, C, D, E, and F (as well as their lowercase counterparts) to represent 10, 11, 12, 13, 14, and 15. <br />


![](Photos/Hexadecimal%20Example.png) <br />
Each hex-digit corresponds to four bits which is half a byte or a nibble.  <br />
A byte can be represented by two hex-digits instead of 8 bits, and a 32-bit word can be written with only 8 hex-digits.
## Decimal Conversion to Hexadecimal
1) Divide the number by 16
2) Get the quotient for the next iteration
3) Get the remainder for the hex digit
	- To get the remainder for the hex digit, multiply the remainder by 16
	- ![](Photos/Find%20Remainder%20Decimal%20for%20the%20Remainder%20Hex.png)
4) Repeat the steps until the quotient is equal to 0.
### Example:
7562<sub>10</sub> to hex
![](Photos/Decimal%20to%20Hexadecimal%20Example.png) <br />
7562<sub>10</sub> = 1D8A<sub>16</sub> 

[Helpful Guide for Converting Decimal to Hexadecimal](https://www.binaryhexconverter.com/decimal-to-hex-converter)

## Hexadecimal Conversion to Decimal 
![](Photos/Hexadecimal%20to%20Decimal%20equation.png) <br />
### Example 1
![](Photos/Hexa%20to%20Decimal%20Example%201.png) <br />
### Example 2 (More Understandable Example)
![](Photos/Hexadecimal%20to%20Decimal%20Example%202.png) <br />

[Helpful Guide for Converting Hexadecimal to Decimal](https://www.binaryhexconverter.com/hex-to-decimal-converter)

## Binary Conversion to Hexadecimal 
Each 4 bit cluster corresponds to a single hex digit. <br />
![](Photos/Binary%20to%20Hexadecimal%20Examples.png) <br />

[Helpful Guide for Converting Binary to Hexadecimal](https://www.rapidtables.com/convert/number/binary-to-hex.html)
# Octal System
This system is now out of date due to the hexadecimal system. But it used to be widespread when many computers used 6 bit bytes, as they tend to be conveniently written as a 2 digit octal number.
![](Photos/Octal%20System%20Examples.png) <br />

To convert binary to octal, every **3 bit cluster** responds to a single octal digit.
If the number of bits in the binary integer is not a multiple of 3, add zeros to the left.<br />
![](Photos/Binary%20to%20Octal%20example.png) <br />
[More on Octal System](https://byjus.com/maths/octal-number-system/)
# Representing Negative Numbers
A single bit is used to represent the sign of the number (+ or -) and the remaining bits to represent the  magnitude of the number (how positive or negative it is).  
The most common representation of positive and negative integers is two's complement. In two's complement, positive integers are represented in standard binary, as in signed magnitude. 

### How to represent a Negative Number to Binary
1) Find the binary representation of the magnitude of number (the positive version of the negative number)
	- **Example:** -13 -> 00001101
2) Inverse the numbers
	- **Example:** 00001101 -> 11110010
3) Add 1
	- **Example:** 11110010 -> 11110011

The **most-significant bit** of 1 signifies a negative number, but the rest of the bits do not encode the magnitude in the regular way.
![](Photos/Most-Significant%20Bit%20Example.png)
### How to Convert Binary Back to a Negative Decimal
1) Inverse all the bits
	- **Example:** 10010110 -> 01101001
2) Add 1
	- **Example:** 01101001 -> 01101010
2) Interpret the result as a binary representation (find the positive number) of the magnitude then add a negative sign.
	- **Example:** 01101010 -> 106 -> -106