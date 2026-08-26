Made by: Leigh Aldrie Dumapias | 2ECE-D

This repository contains the Programming Assignment 1 assigned for ECE2112 - Advanced Computer Programming & Algorithms for A.Y. 2026 - 2027. The project includes three specific Python problems intended for utilization of basic Python skills.

## 1. Word Rotation Problem

Objective:

To create a function named "rotate_word()" that accepts a non-empty string value and moves the first character of the string in the end while keeping the other elements in place. Capitalization of every character must also be preserved. String indexing or slicing must be utilized to construct the returned string.

Key Components:

• `def rotate_word(text):` - a user-defined function, the included `text` acts as a placeholder for whatever string that it is passed into the function.

• `text[1:]` - a built-in process that that slices the characters of the string from the index position 1 all the way to the last.

• `text[0]` - a built-in process that only gets the character from the index position zero

• `return text[1:] + text[0]` - the two is combined by "+" that will put character of index position zero at last without changing others' position, then `return` will give out the output.

The final output is built as follows: 

```python
def rotate_word(text):
    
    return text[1:] + text[0]

print(rotate_word("Python"))
```

## 2. Username Builder Problem

Objective:

To create a function named make_username() that accepts two strings: first name and last name. The
function must convert all letters to lowercase, remove all spaces from the first name and last name. Then, the processed first and last names must be joined together using one period (.).

Key Components:

• `def make_username(first_name, last_name):` - a user-defined function, the included `first_name, last_name` acts as a placeholder for whatever string that it is passed into the function.

• `lowercase_first = first_name.lower()` - the `first_name.lower()` has the built-in process `.lower()` that converts all the elements placed in the `first_name` to lowercase, and then stores the new value to the placeholder `lowercase_last`.

• `final_first = lowercase_first.replace(" ","")` - the `lowercase_first.replace(" ", "")` has the built-in process `.replace()`, in this case, coded to be `.replace(" ","")` that helps in replacing certain elements in the input. Inside the parenthesis, the first one between the double quotation mark is a space, that means the process will search for spaces in the value placed in `lowercase_first`, then, the second part inside the parenthesis, that is also enclosed by double quotation mark have no space, which is the condition that will replace the scanned spaces in the first one, resulting to removal of any space. Then, after this process, it will store the result value in the placeholder `final_first`.

• `lowercase_last = last_name.lower()` - the `last_name.lower()` has the built-in process `.lower()` that converts all the elements placed in the `last_name` to lowercase, and then stores the new value to the placeholder `lowercase_last`.

• `final_last = lowercase_last.replace(" ","")` - the `lowercase_last.replace(" ", "")` has the built-in process `.replace()`, in this case, coded to be `.replace(" ","")` that helps in replacing certain elements in the input. Inside the parenthesis, the first one between the double quotation mark is a space, that means the process will search for spaces in the value placed in `lowercase_last`, then, the second part inside the parenthesis, that is also enclosed by double quotation mark have no space, which is the condition that will replace the scanned spaces in the first one, resulting to removal of any space. Then, after this process, it will store the result value in the placeholder `final_last`.

• `return final_first + "." + final_last` - the stored values in `final_first` and `final_last` will be joint together by operation "+", then between them a period is also place with `"."`. Then `return` will give out the output.

The final output is built as follows:

```python
def make_username(first_name, last_name):

    lowercase_first = first_name.lower()

    final_first = lowercase_first.replace(" ","")

    lowercase_last = last_name.lower()

    final_last = lowercase_last.replace(" ","")

    return final_first + "." + final_last

print(make_username("Leigh","Aldrie"))
```

## 3. Bookend Swap Problem

Objective:

To create a function named swap_bookends() that accepts a list containing at least two elements. Unpack the list into three variables:

• first – the first element;

• middle – a list containing everything between the first and last elements; and

• last – the last element.

Using these variables, return a new list in which the first and last elements have exchanged positions. The elements in middle must remain in their original order.

Key Components:

• `def swap_bookends(items):` - creates a user-defined function, the "items" is an input passed in the function, which is expected to be a list containing at least two elements.

• `first, *middle, last = items` 

- "first" takes the first element in "items" list and stores it in the variable
  
- "*middle" possessing an asterisk to capture all the remaining elements in between the first and last elements of the "items" list, grouping it in a new list
  
- "last" takes the last element in "items" list and stores it in the variable

• `return [last] + middle + [first]`

- [last] wraps the single last elements to be a list
  
- [first] wraps the single first element to be a list

- middle joins both the "last" and the "first" list with the help "+". Does not need to be put in a squared bracket because it already declared to be a list in the previous line of code. The newly constructed list is then returned by `return`.

The final output is built as follows:

```python
def swap_bookends(items):

    first, *middle, last = items

    return [last] + middle + [first]
    
swap_bookends([1, 2, 3, 4, 5])
```

To see the main python program for Programming Assignment 1, the link is given by https://github.com/leighaldriedumapias/ECE-2112-PA-1/blob/master/Programming%20Assignment%201.ipynb and download. Open on Jupyter Notebook, then run all cells.

## README File Version History:

August 26, 2026 - Initial README output uploaded; also format and details tweaks
