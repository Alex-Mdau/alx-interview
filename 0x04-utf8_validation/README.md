UTF-8 Validation

This repository contains a Python script to determine if a given data set represents a valid UTF-8 encoding.
Task

The task is to implement a method called validUTF8(data) that takes a list of integers as input and checks whether it represents a valid UTF-8 encoding. The method should return True if the data is a valid UTF-8 encoding, otherwise, it should return False.
Requirements

    A character in UTF-8 can be 1 to 4 bytes long.
    The data set can contain multiple characters.
    Each integer in the list represents 1 byte of data, so only the 8 least significant bits of each integer need to be handled.

How to Use

    Clone this repository to your local machine or download the 0-validate_utf8.py file.

    Ensure you have Python installed on your machine.

    Open a terminal or command prompt and navigate to the directory where the 0-main.py and 0-validate_utf8.py files are located.

    Run the 0-main.py script using the following command:

    css

    python3 0-main.py

Example

Below are some example usages of the validUTF8(data) method:

python

data = [65]
print(validUTF8(data))  # Output: True

data = [80, 121, 116, 104, 111, 110, 32, 105, 115, 32, 99, 111, 111, 108, 33]
print(validUTF8(data))  # Output: True

data = [229, 65, 127, 256]
print(validUTF8(data))  # Output: False

