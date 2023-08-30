


## Making Change

This program takes in a list of coins and a total amount, and returns the fewest number of coins needed to make that amount.

### Code Explanation

The code is split into two files:

* `0-main.py`: This file imports the `makeChange` function from the `0-making_change.py` file and tests it with two different inputs.
* `0-making_change.py`: This file contains the `makeChange` function, which takes in a list of coins and a total amount, and returns the fewest number of coins needed to make that amount.

The `makeChange` function works by first sorting the list of coins in descending order. This makes it easier to find the largest coin that can be used to make change for the total amount. The function then iterates through the list of coins, starting with the largest coin. For each coin, the function checks if the total amount is greater than or equal to the coin's value. If it is, the function increments a counter and subtracts the coin's value from the total amount. The function continues iterating through the list of coins until the total amount is zero. If the total amount is zero, the function returns the counter. If the total amount is not zero, the function returns -1.

### Example Usage

The following code shows how to use the `makeChange` function:

```python
import makeChange

coins = [1, 2, 25]
total = 37

print(makeChange(coins, total))
```

This code will print the following output:

```
4
```

This means that it takes 4 coins to make 37 cents.

### Step-by-Step Explanation

The following is a step-by-step explanation of how the `makeChange` function works:

1. The function sorts the list of coins in descending order.
2. The function initializes a counter to 0.
3. The function iterates through the list of coins, starting with the largest coin.
4. For each coin, the function checks if the total amount is greater than or equal to the coin's value.
5. If the total amount is greater than or equal to the coin's value, the function increments the counter and subtracts the coin's value from the total amount.
6. The function continues iterating through the list of coins

