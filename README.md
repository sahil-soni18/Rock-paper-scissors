# Rock-paper-scissors
print("WELCOME TO THE ROCK, PAPER AND SCISSORS GAME!!")
list = ["rock","paper","scissors"]
print("how many time you want to play:")
p=int(input())
import random
t=1
user_score=0
CPU_score=0
while(t<=p):
    print("choose 1. rock\n 2. paper\n 3. scissors.")
    user_choice = input()
    CPU_choice = random.choice(list)
    print("CPU chose",CPU_choice)
    if user_choice == "rock" and CPU_choice == "paper":
        print("BETTER LUCK NEXT TIME")
        CPU_score += 1
        print("you = ", user_score, "CPU = ", CPU_score)
        t+=1
    elif user_choice == "paper" and CPU_choice == "rock":
        print("YOU WON THE ROUND!")
        user_score += 1
        print("you = ", user_score, "CPU = ", CPU_score)
        t+=1
    elif user_choice == "paper" and CPU_choice == "scissors":
        print("BETTER LUCK NEXT TIME")
        CPU_score += 1
        print("you = ", user_score, "CPU = ", CPU_score)
        t+=1
    elif user_choice == "scissors" and CPU_choice == "paper":
        print("YOU WON THE ROUND!")
        user_score += 1
        print("you = ", user_score, "CPU = ", CPU_score)
        t+=1
    elif user_choice == "rock" and CPU_choice == "scissors":
        print("YOU WON THE ROUND!")
        user_score += 1
        print("you = ", user_score, "CPU = ", CPU_score)
        t+=1
    elif user_choice == "scissors" and CPU_choice == "rock":
        print("BETTER LUCK NEXT TIME")
        CPU_score += 1
        print("you = ", user_score, "CPU = ", CPU_score)
        t+=1
    else:
        print("ROUND TIE!!")
        print("you = ", user_score, "CPU = ", CPU_score)

print("ROUNDS ARE OVER!!\n you ",user_score, " CPU ",CPU_score)
if user_score>CPU_score:
    print("WINNER WINNER CHICKEN DINNER!!")
elif CPU_score>user_score:
    print("OOPS!! CPU WON THE GAME.")
else:
    print("GAME TIE!!")
