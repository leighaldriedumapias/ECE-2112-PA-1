Made by: Leigh Aldrie Dumapias | 2ECE-D

This repository contains the Programming Assignment 1 assigned for ECE2112 - Advanced Computer Programming & Algorithms for A.Y. 2026 - 2027. The project includes three specific Python problems intended for utilization of basic Python skills.

## 1. Word Rotation Problem

Objectives:

To create a function named "rotate_word()" that accepts a non-empty string value and moves the first character of the string in the end while keeping the other elements in place. Capitalization of every character must also be preserved. String indexing or slicing must be utilized to construct the returned string.

Key Components:

• `def rotate_word(text):` - a user-defined function, the included `text` acts as a placeholder for whatever string that it is passed into the function.

• `text[1:]` - a built-in process that that slices the characters of the string from the index position 1 all the way to the last.

• `text[0]` - a built-in process that only gets the character from the index position zero

• `return text[1:] + text[0]` - the two is combined by "+" that will put character of index position zero at last without changing others' position, then `return` will give out the output.

The final output is built as follows: 

```
def rotate_word(text):
    
    return text[1:] + text[0]

print(rotate_word("Python"))
```    
