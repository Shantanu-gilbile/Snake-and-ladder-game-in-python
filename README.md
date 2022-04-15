# Snake-and-ladder-game-in-python

"""
Snake and ladeer game
created by Shantanu Gilbile
using just simple concept of python
and random module.
"""

import random

print("Start the Game !!!")

player = [0,0]

i=0

print("Ladder at positions 4 , 16 , 26 and 36")

print("Snake position at 11 , 28 , 37 and 48")

while (player[0]!=50 and player[1]!=50):

    print("player ",i+1," Turns")
    player[i]+=random.randint(1,6)

    if (player[i]==4 or player[i]==16 or player[i]==26or player[i]==36):

        print("Yeeess got a lader !!!")

        if(player[i]==4):
            player[i]=15

        if(player[i]==16):
            player[i]=27

        if(player[i]==26):
            player[i]=34

        if(player[i]==36):
            player[i]=47

    if (player[i] == 11 or player[i] == 28 or player[i] == 37 or player[i] == 48):

        print("hii, Snakeee here !!!")
        
        if (player[i] == 11):
            player[i] = 9

        if (player[i] == 28):
            player[i] = 14

        if (player[i] == 37):
            player[i] = 20

        if (player[i] == 48):
            player[i] = 3

    i=(i+1) % 2  #to change the from player 1 to player 2

if(player[0]==50):

    print("Congratulation to player 1")

if(player[1]==50):

    print("Congratulation to player 2")




