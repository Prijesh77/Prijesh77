import random
while True:

    choices= ["rock", "paper", "scissors"]

    comp= random.choice(choices)
    player= None

    while player not in choices:
        player= input("rock, paper, scissors?:").lower()

    if comp==player :
        print("computer: "+comp)
        print("player: "+player)
        print("tie!")
    elif player== "rock":
        if comp== "paper":
            print("computer: " + comp)
            print("player: " + player)
            print("You lose!")
        if comp== "scissors":
            print("computer: " + comp)
            print("player: " + player)
            print("You win!")
    elif player == "scissors":
        if comp == "rock":
            print("computer: " + comp)
            print("player: " + player)
            print("You lose!")
        if comp == "paper":
            print("computer: " + comp)
            print("player: " + player)
            print("You win!")
    elif player == "paper":
        if comp == "scissors":
            print("computer: " + comp)
            print("player: " + player)
            print("You lose!")
        if comp == "rock":
            print("computer: " + comp)
            print("player: " + player)
            print("You win!")
        play_again= input("Do you want to play again ? (yes/no):").lower()

        if play_again != "yes":
            break
print("bye!")
