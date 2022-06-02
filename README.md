# rock-paper-and-scissors-zuri-task
import random

while True:

    possible_option = ["rock","paper","scissors"]
    computer = random.choice(possible_option)

    player = None

    while player not in possible_option:
        player = input("Rock, Paper, Scissors: ").lower()

    if player == computer:
        print(f"Computer({computer})")
        print(f"Player({player})")
        print("This is a Tie")
    elif player == "rock":
        if computer == "paper":
            print(f"Computer({computer})")
            print(f"Player({player})")
            print("Sorry! You Lose")
        if computer == "scissors":
            print(f"Computer({computer})")
            print(f"Player({player})")
            print("Congrats! You Won")

    elif player == "scissors" and "s":
        if computer == "rock":
            print(f"Computer({computer})")
            print(f"Player({player})")
            print("Sorry! You Lose")
        if computer == "paper":
            print(f"Computer({computer})")
            print(f"Player({player})")
            print("Congrats! You Won")

    elif player == "paper" and "p":
        if computer == "scissors":
            print(f"Computer({computer})")
            print(f"Player({player})")
            print("Sorry! You Lose")
        if computer == "rock":
            print(f"Computer({computer})")
            print(f"Player({player})")
            print("Congrats! You Won")

    play_again = input("Play again? (yes/no):").lower()

    if play_again != "yes":
        break

print("Game has ended!")
