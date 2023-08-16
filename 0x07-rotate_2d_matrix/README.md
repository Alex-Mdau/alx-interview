The following code rotates a 2D matrix 90 degrees clockwise. The matrix is edited in-place.

```python
def rotate_2d_matrix(matrix):
    """
       Rotates 2D matrix 90 degrees clockwise
       Matrix is edited in-place
       args:
          matrix
    """
    left, right = 0, len(matrix) - 1

    while left < right:
        for i in range(right - left):
            top, bottom = left, right
            # save topleft  value
            topLeft = matrix[top][left + i]
            # move bottom left to top left
            matrix[top][left + i] = matrix[bottom - i][left]
            # move bottom right to bottom left
            matrix[bottom - i][left] = matrix[bottom][right - i]
            # move top right to bottom right
            matrix[bottom][right - i] = matrix[top + i][right]
            # move top left to top right
            matrix[top + i][right] = topLeft
        right -= 1
        left += 1
```

The function first defines two variables, `left` and `right`, which represent the left and right edges of the matrix, respectively. The function then enters a while loop that iterates over the matrix from left to right. Within the loop, the function iterates over the rows of the matrix from top to bottom, saving the value of the top-left element in a variable called `topLeft`. The function then moves the bottom-left element to the top-left position, the bottom-right element to the bottom-left position, the top-right element to the bottom-right position, and the top-left element to the top-right position. The function then decrements `right` and increments `left`, which ensures that the next iteration of the loop will process the next row of the matrix.

The function returns once the entire matrix has been rotated.