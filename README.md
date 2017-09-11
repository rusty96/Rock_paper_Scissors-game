# Rock_paper_Scissors-game
It's a simple Python(3.6.2) code for Rock_paper_Scissors game
Code:
#!/bin/python3
from random import randint
player = input('rock(r), paper(p), scissors(s)?')
#print(player,'vs' , end='')
if player == 'r':
    print('0', end='')
elif player == 'p':
    print('_', end='')
elif player == 's':
    print('>8', end='')
chosen = randint(1,3)
#print(chosen)
if chosen == 1:
    computer = 'r'
    print('0')
elif chosen == 2:
    computer = 'p'
    print('_')
else:
    computer = 's'
    print('>8')
#print(computer)
if player == computer:
    print('Draw!')
elif player == 'r' and computer == 's':
    print('Player Wins!')
elif player == 'r' and computer == 'p':
    print('Computer Wins!')
elif player == 'p' and computer == 'r':
    print('Player Wins!')
elif player == 'p' and computer == 's':
    print('Computer Wins!')
elif player == 's' and computer == 'p':
    print('Player Wins!')
elif player == 's' and computer == 'r':
    print('Computer Wins!')

