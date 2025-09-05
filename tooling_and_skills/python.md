---
layout: default
---

# Python Data Structures Cheat Sheet

## Types of Data Structures in Python

### Python Primitive Data Structures

These store simple data values.

| Description |                                                                         | Examples         |
|-------------|-------------------------------------------------------------------------|------------------|
| String      | Collection of characters surrounded by single or double quotation marks | 'Alice', "Bob"   |
| Boolean     | Logical values                                                          | True, False      |
| Integer     | Whole number of unlimited length                                        | 0, -273          |
| Float       | Floating-point decimal                                                  | 1.618, 3.1415926 |

### Python Built-In Non-Primitive Data Structures

These data structures, which store values and collections of values, are inherent to Python.

| Description                                     | Ordered         | Allow duplicates | Mutable | Syntax       | Examples                                                                               |
|-------------------------------------------------|-----------------|------------------|---------|--------------|----------------------------------------------------------------------------------------|
| List                                            | √               | √                | √       | [ ]          | • [1, 2.3, True] • ['John', 'Doe']                                                     |
| Tuple                                           | √               | √                | ✕       | ( )          | • ('age', 22) • (7.89, False)                                                          |
| Set  0 is the same as False, as are 1 and True. | ✕               | ✕                | ✕       | { }          | • {6, 4.5} • {'nice', True}                                                            |
| Dictionary  Map, storing key-value pairs.       | √ > 3.7 ✕ ≤ 3.6 | ✕                | √       | {key: value} | • {"FB": "Facebook", "WA": "WhatsApp", "IG": "Instagram"} • {'name': 'Bob', 'id': 255} |

## List and Tuple Operations

### Accessing Items in Lists

The table below is based on this list:

fruit_list = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"].

| Command                                                       | Description                                                            |
|---------------------------------------------------------------|------------------------------------------------------------------------|
| fruit_list[0]                                                 | Get the first item on the list ("apple")                               |
| fruit_list[1]                                                 | Get the second item on the list ("banana")                             |
| fruit_list[-1]                                                | Get the last item ("mango")                                            |
| fruit_list[­2:5]                                              | Get the items from start to end indexes                                |
| fruit_list[:4]                                                | Get the items from the beginning but exclude "kiwi" and beyond         |
| fruit_list[2:]                                                | Get the items from "­che­rry­" to the end                              |
| fruit_list[­-4:-1]                                            | Get the items from "­ora­nge­" (-4) onwards but exclude "­man­go" (-1) |
| if "­app­le" in fruit_list:    print(­"Yes, we have 'apple'") | Check if "­app­le" is in the list                                      |

### List (and Tuple) Methods

Commands with an asterisk (*) apply to tuples.

| Command                     | Description                                                                  | Usage                                                                             |
|-----------------------------|------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|
| append()                    | Add an element at the end of the list                                        | list1.a­ppend(element)                                                            |
| clear()                     | Remove all the elements from the list                                        | list1.c­lear()                                                                    |
| copy()                      | Return a copy of the list                                                    | list1.c­opy()                                                                     |
| count()                     | Return the number of elements with the specified value*                      | list1.c­oun­t(e­lement)                                                           |
| extend()                    | Add the elements of a list (or any iterable), to the end of the current list | list1.e­xt­end­(list2)                                                            |
| index()                     | Return the index of the first element with the specified value*              | list1.i­nde­x(e­lem­ent­[,s­tar­t[,­end]])                                        |
| insert()                    | Add an element at the specified position (position is an integer)            | list1.i­nse­rt(­po­sition, element)                                               |
| pop()                       | Remove the element at the specified position                                 | list1.p­op(­[in­dex])                                                             |
| remove()                    | Remove the first item with the specified value                               | list1.r­emo­ve(­ele­ment)                                                         |
| reverse()                   | Reverse the order of the list                                                | list1.re­verse()                                                                  |
| sort() sort(reverse = True) | Sort the list in ascending / descending order                                | list1.sort() list2.sort(reverse = True)                                           |
| del()                       | Delete from the list the item specified with its index                       | del list1[­index]                                                                 |
| list1 + list2               | Join two lists                                                               | list1 = ["x", "y"] list2 = [8, 9] list3 = list1 + list2  # Returns: ["x","y",8,9] |

### List Comprehension

List comprehension simplifies the creation of a new list based on the values of an existing list.

| Command                                                  | Description                                          |
|----------------------------------------------------------|------------------------------------------------------|
| [n for n in range(10) if n < 5]                          | Accept only numbers less than 5                      |
| [x for x in fruits if "­a" in x]                         | Accept items containing "­a".                        |
| [x for x in fruits if x != "­app­le"]                    | Accept all items except "­app­le"                    |
| [x.upper() for x in fruits]                              | Make uppercase the values in the new list            |
| [x + '?' for x in fruits]                                | Add a question mark at the end of each item          |
| ['hello' for x in fruits]                                | Set all values in the new list to 'hello'            |
| [x if x != "­ban­ana­" else "­ora­nge­" for x in fruits] | Replace "­ban­ana­" with "­ora­nge­" in the new list |

### Accessing Items in Tuples

Below, the tuple in question is fruits = ("apple", "banana", "cherry").

### Tuple Manipulation

### Adding items

You can add items to a tuple as follows:

Tip: When creating a single-item tuple, remember to include a comma.

### Removing items and changing values

Since tuples are immutable, you can’t remove or modify their contents directly. The key is converting it into a list and back.

## Dictionary Operations

### Adding Items

There are three methods

Warning: duplicate keys will cause the latest values to overwrite earlier values.

### General Operations

## Set Operations

### Accessing

Although you can’t directly access items in a set, you can loop through the items:

### Adding and Removing Items

### Mathematical Operations

## Algorithms and the Complexities

This section is about the complexity classes of various Python data structures.

### List

Tuples have the same operations (non-mutable) and complexities.

### Dictionary

### Set

## Symbol Table

Python keeps track of variables using symbol tables, which you can explore using the following basic commands:

## Python Libraries

The following commands are for setting up Python programs or libraries for use inside your program:

Examples of [Python libraries](https://docs.python.org/3/library/) containing other non-primitive data structures:

* array: Efficient arrays of numeric values
* collections: Abstract data structures
* dataclasses: For creating user-defined data structures
* datetime: Basic date and time types
* queue: Synchronized queue class

[Back](/tools_and_skills.html)