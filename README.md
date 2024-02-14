# Thinkthenumber
In this game, the computer picks a random number between two other numbers, If you want to learn how to make this game using Python, this article can help you. It will show you step by step how to write the code for the game.To make the guessing game, we need to write a program that chooses a random number between 1and 10.
import random

n = random.randrange(1, 10)
guess = int(input("Enter the number: "))

while n != guess:
    if guess < n:
        print("Too low")
        guess = int(input("Enter the number again: "))
    elif guess > n:
        print("Too high")
        guess = int(input("Enter the number again: "))
    else:
        break

print("You guessed correctly!")
