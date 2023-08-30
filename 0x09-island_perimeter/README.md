 ```
# Island Perimeter

This code calculates the perimeter of an island. An island is a group of connected 1s in a grid of 0s. The perimeter is the number of 1s that are adjacent to a 0.

## Step-by-step explanation

The code is divided into two files:

* `0-island_perimeter.py`: This file contains the function that calculates the perimeter of an island.
* `0-main.py`: This file imports the function from `0-island_perimeter.py` and calls it to calculate the perimeter of a given island.

The function `island_perimeter()` takes a grid as input and returns the perimeter of the island. The grid is a list of lists, where each inner list represents a row in the grid. The function works by iterating over each element in the grid and checking if it is a 1. If it is, the function increments the perimeter by 4. However, if the element is adjacent to another 1, the function decrements the perimeter by 2. This is because the perimeter of an island only includes the 1s that are adjacent to a 0.

The function `main()` imports the function `island_perimeter()` from `0-island_perimeter.py` and calls it to calculate the perimeter of a given island. The island is represented by a list of lists, where each inner list represents a row in the grid. The function prints the perimeter of the island to the console.

## Example

The following is an example of how to use the code to calculate the perimeter of an island:

```python
grid = [
    [0, 0, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0],
    [0, 1, 1, 1, 0, 0],
    [0, 0, 0, 0, 0, 0]
]

perimeter = island_perimeter(grid)

print(perimeter)
```

The output of the code is:

```
16
```

This means that the perimeter of the island is 16.



