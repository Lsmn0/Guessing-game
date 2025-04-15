# Guessing-game
import random
winning_no = random.randint(1,100)
guess = 1

while True:
    try:
        user_input = int(input("Enter the number from 1 to 100: "))

    except ValueError:
        print("Please enter the number from 1 to 100")
        continue

    if user_input == winning_no:
        print(f"Congrats you guess correct {guess} times")
        break

    else:
        if user_input > winning_no:
            print("Guess no is too high")
        else:
            print("Guess no is too low")
    guess+=1
