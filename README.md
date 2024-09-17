# Rock-Paper-Scissors
This is my first python project of udemy's 100 days of code course. This is a Rock-paper-scissor game.
<br>
Author- Debanuj 

import random
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
c=input('Choose your attack (rock, paper or scissors):\n')
if c=='rock':
    print('Your choice:', rock)
elif c=='paper':
    print('Your choice:', paper)
elif c=='scissors':
    print('Your choice:', scissors)
l=[rock, paper, scissors]
a=random.choice(l)
print('The computer chooses:', a)
if c=='rock' and a==scissors:
    print('You Win')
elif c==rock and a==paper:
    print('You lose')
elif c=='paper' and a==scissors:
    print('You lose')
elif c=='paper' and a==rock:
    print('You Win')
elif c=='scissors' and a==paper:
    print('You Win')
elif c=='scissors' and a==rock:
    print('You lose')
else:
    print('It is a draw')
