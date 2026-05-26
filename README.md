# String Encoder Decoder

## Overview

This is a beginner Python project that uses run length encoding to compress repeated characters into tuples and then decode those tuples back into a string.

This project was created to practice Python fundamentals, including functions, loops, conditionals, lists, tuples, string manipulation, and basic data transformation logic.

## Purpose

I built this project as part of my technical preparation for graduate study in Information Systems.

The goal was to practice writing Python functions that process text, transform data, and return a result.

This project is not encryption. It is a basic encoding and decoding exercise that helped me understand how data can be represented in a different format and then reconstructed.

## Project Files

- main.py: contains the encoder and decoder functions
- README.md: explains the project and how to run it

## How to Run This Project

1. Download or clone this repository.
2. Open the project folder in a code editor.
3. Open the file named main.py.
4. Run the file in the terminal.

On Mac, use:

    python3 main.py

On some computers, you may use:

    python main.py

## How to Use the Encoder

The encoder turns repeated characters into tuples.

In main.py, find this line:

    print(encodeString("AAABBBdddd"))

To test your own input, replace "AAABBBdddd" with another word or phrase.

Example:

    print(encodeString("hhheeellooo"))

This will return something like:

    [('h', 3), ('e', 3), ('l', 2), ('o', 3)]

## How to Use the Decoder

The decoder takes tuples and rebuilds the string.

In main.py, find this line:

    print(decodeString([('A', 4), ('b', 8)]))

To test your own input, replace the tuple list with another list of character and count pairs.

Example:

    print(decodeString([('h', 3), ('e', 3), ('l', 2), ('o', 3)]))

This will return:

    hhheeellooo

## Example Output

When you run the project, the output may look like this:

    These are the encoded tuples
    [('A', 3), ('B', 3), ('d', 4)]

    These are the decoded tuples
    AAAAbbbbbbbb

## Skills Practiced

- Python functions
- Loops
- Conditional logic
- Lists
- Tuples
- String manipulation
- Basic encoding and decoding logic
- Debugging and problem solving

## What I Learned

Through this project, I practiced how to process a string one character at a time, track repeated values, store results in a list of tuples, and rebuild a string from structured data.

This helped me better understand how Python can be used to transform and reconstruct information.

## Project Status

Completed as a beginner Python learning project.
