 # 0x0A-primegame

This is a Python program that implements the Prime Game. The game is played between two players, Maria and Ben. The goal of the game is to be the first player to choose a prime number that the other player cannot match.

The program consists of two files:

* `0-prime_game.py`: This file contains the implementation of the game logic.
* `main_0.py`: This file contains the main function that runs the game.

## 0-prime_game.py

The `primeNumbers` function returns a list of prime numbers between 1 and `n` inclusive. The function uses the Sieve of Eratosthenes algorithm to find prime numbers. The algorithm works by first creating a list of all numbers from 2 to `n`. Then, the algorithm iterates through the list and marks all multiples of each number as composite. The numbers that are not marked as composite are prime numbers.

The `isWinner` function determines the winner of the Prime Game. The function takes two arguments: `x`, the number of rounds of the game, and `nums`, a list of the upper limits of the range for each round. The function returns the name of the winner (Maria or Ben) or `None` if there is no winner.

The function works by first finding the list of prime numbers for each round of the game. Then, the function iterates through the list of prime numbers and increments the score of the player who chose the prime number. The player with the highest score at the end of the game is the winner.

## main_0.py

The `main` function runs the Prime Game. The function first prompts the user for the number of rounds of the game and the upper limits of the range for each round. Then, the function calls the `isWinner` function to determine the winner of the game. Finally, the function prints the name of the winner to the console.

## Usage

To run the Prime Game, follow these steps:

1. Clone the repository.
2. Install Python 3.
3. Run the following command:

```
python3 main_0.py
```

4. Enter the number of rounds of the game and the upper limits of the range for each round.
5. The program will print the name of the winner to the console.



