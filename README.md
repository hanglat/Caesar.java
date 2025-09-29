# Caesar Cipher (Java)

This project implements a simple **Caesar cipher** in Java.  
It takes a shift key `K` as the first command-line argument and one or more messages as additional arguments.  
Uppercase and lowercase letters are shifted within the alphabet, while non-letter characters remain unchanged.  

## Usage
```bash
javac Caesar.java
java Caesar 3 Hello World

Output:

Khoor
Zruog

Features:

   - Works with multiple input messages

   - Preserves case (uppercase/lowercase)

   - Leaves non-letter characters unchanged

Example:

java Caesar 5 Programming IsFun

Output:

Uwtlwfrrnsl NxKzs

Notes:

   - Implemented in pure Java, no external libraries required.

   - Great example for string manipulation, loops, and command-line arguments.
