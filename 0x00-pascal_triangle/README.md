# Pascal's Triangle

This directory  contains a Python function `pascal_triangle(n)` that generates Pascal's triangle of `n` rows. It returns a list of lists of integers representing the triangle.

## Function Description

```python
def pascal_triangle(n):
    """
    Generate Pascal's triangle of n rows.

    Args:
        n (int): The number of rows in the triangle.

    Returns:
        list: List of lists of integers representing Pascal's triangle.

    """

The function takes an integer n as input and returns the corresponding Pascal's triangle. If n is less than or equal to 0, it returns an empty list.
Usage

Here's an example usage of the pascal_triangle() function:

python

from pascal_triangle import pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))

if __name__ == "__main__":
    print_triangle(pascal_triangle(5))

The above example will output:

csharp

[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]

Repository Structure

    GitHub repository: alx-interview
    Directory: 0x00-pascal_triangle
    File: 0-pascal_triangle.py
