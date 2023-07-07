# lockboxes

## Description
This directory contains a Python implementation of a method called `canUnlockAll` that determines whether all the boxes in a given list can be opened. Each box is numbered sequentially from 0 to n - 1, and a box may contain keys to the other boxes.

## Method Signature
```python
def canUnlockAll(boxes)

Method Details

    boxes is a list of lists.
    A key with the same number as a box opens that box.
    You can assume all keys will be positive integers.
    There can be keys that do not have boxes.
    The first box boxes[0] is unlocked.
    The method returns True if all boxes can be opened, and False otherwise.

Algorithm

The canUnlockAll method uses a breadth-first search approach to determine if all the boxes can be unlocked. It maintains a list called unlocked to keep track of whether each box is unlocked or not. Initially, all boxes are marked as locked except for the first box (boxes[0]).

The algorithm starts by adding all the keys from the first box to a set called keys. Then, it enters a loop that continues until there are no more keys to process. In each iteration, it pops a key from the keys set, unlocks the corresponding box by setting unlocked[box] to True, and updates the keys set by adding any new keys found in the unlocked box, excluding keys that are already accounted for or duplicates.

After processing all the keys, the algorithm checks if all the boxes are unlocked by using the all function on the unlocked list.
Usage Example

python

boxes = [[1], [2], [3], []]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 2], [3], [1, 4], []]
print(canUnlockAll(boxes))  # Output: False

