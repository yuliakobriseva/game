# game
import random

def roll_dice():
    return random.randint(1, 6)

def play_game():
    print("Welcome to the Dice Rolling Game!")
    input("Press Enter to roll the dice...")

    player_roll = roll_dice()
    computer_roll = roll_dice()

    print(f"You rolled: {player_roll}")
    print(f"Computer rolled: {computer_roll}")

    if player_roll > computer_roll:
        print("Congratulations! You win!")
    elif player_roll < computer_roll:
        print("Sorry, the computer wins.")
    else:
        print("It's a tie!")

# Example usage
if __name__ == "__main__":
    play_game()
