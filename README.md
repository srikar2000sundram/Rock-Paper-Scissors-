# Rock-Paper-Scissors-
This is game of Rock Paper and Scissors using python.
#Here We will be using Random function & we will be playing against computer
import random

def play():
  User_Name = input("Enter Your Name")

  user = input(F"What's Your Choice {User_Name} , 'R' for rock, 'P' for paper , 'S' for Scissors")
  computer = random.choice(['R','P','S'])

  if user == computer :
    return " UUUff, It's Tie "
  
  if is_win (user, computer):
    return 'You Won!!!'

  else:
   return 'You Lost , Loser!!!'


def is_win(player, opponent):
    if ( player == 'R' and opponent == 'S') or ( player == 'S'  and  opponent == 'P') or (player == 'P' and opponent == 'S' ) :
       return True

print(play())
