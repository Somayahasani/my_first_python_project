# my_first_python_project
import random
while True:
    choice = ("r", "s", "p")
    user_choice = input("Choose: Rock, Scissor, Paper (r/p/s):")
    if user_choice not in choice:
       print("Invalid number")
       break
    computer_choice = random.choice(choice)
    if computer_choice == user_choice:
        print("tie")
    elif (computer_choice == "r" and user_choice == "s" or
    computer_choice == "s" and user_choice == "p" or
    computer_choice == "p" and user_choice == "r"):
     print("Computer win!")
    else:
     print("You win!")
    should_continue = input("Continue: (Y/N):")
    if should_continue == "N,":
       break
