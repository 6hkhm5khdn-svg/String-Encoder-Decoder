# String Encoder Decoder

## Overview

This is a beginner Python project that uses run length encoding to compress repeated characters into tuples and then decode those tuples back into a string.

This project was created to practice Python fundamentals, including functions, loops, conditionals, lists, tuples, string manipulation, file handling, and basic data transformation logic.

## Purpose

I built this project as part of my technical preparation for graduate study in Information Systems.

The goal was to practice writing Python functions that process text, transform data, return a result, and work with basic file input and output.

This project is not encryption. It is a basic encoding and decoding exercise that helped me understand how data can be represented in a different format and then reconstructed.

## Project Files

main.py: contains the encoder, decoder, file encoder, and file decoder functions.

README.md: explains the project and how to run it.

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

## How to Use the File Encoder

This project also includes a file based encoder.

The function:

    encodeFile(filename, newFilename)

reads a text file, encodes the contents, and saves the encoded version to a new file.

### Example

Create a text file in the same folder called:

    sample.txt

Put text inside it, such as:

    AAABBBdddd

Then add this line at the bottom of main.py:

    encodeFile("sample.txt", "encoded.txt")

Run the file:

    python3 main.py

This will create a new file called:

    encoded.txt

The encoded file will contain the tuple version of the text.

## How to Use the File Decoder

The file decoder reads an encoded file and returns the decoded original text.

The function:

    decodeFile(filename)

reads the encoded file and rebuilds the original string.

### Example

After creating encoded.txt, add this line at the bottom of main.py:

    print(decodeFile("encoded.txt"))

Run the file again:

    python3 main.py

This will print the decoded original text.

## Example Output

When you run the basic encoder and decoder examples, the output may look like this:

    These are the encoded tuples
    [('A', 3), ('B', 3), ('d', 4)]

    These are the decoded tuples
    AAAAbbbbbbbb

## Skills Practiced

Python functions

Loops

Conditional logic

Lists

Tuples

String manipulation

File reading

File writing

Basic encoding and decoding logic

Debugging and problem solving

## What I Learned

Through this project, I practiced how to process a string one character at a time, track repeated values, store results in a list of tuples, and rebuild a string from structured data.

I also practiced basic file handling by reading text from one file, encoding it, writing the encoded output to another file, and decoding the saved file back into readable text.

This helped me better understand how Python can be used to transform, store, and reconstruct information.

## Project Status

Completed as a beginner Python learning project.
