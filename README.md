# PYTHON-PROJECTS
#ROCK PAPER AND SCISSOR GAME


import random
def game (comp,you):
    if comp==you:
        return None
    elif comp=='r':
        if you=='s':
            return False
        elif you=='p':
            return True
    elif comp=='p':
        if you=='s':
            return True
        elif you=='r':
            return False
    elif comp=='s':
        if you=='p':
            return False
        elif you=='r':
            return True
print("Comp Turn: Rock(r) Paper(p) Scissor(s) ")
randNo=random.randint(1,3)
if randNo==1:
    comp='r'
elif randNo==2:
    comp='p'
elif randNo==3:
    comp='s'

you= input("Your Turn: Choose Rock(r) Paper(p) and Scissor(s)")
print(f"Comp chose {comp}")
print(f"You chose {you}")

x= game(comp,you)

if x==None:
    print("The game is a tie")
elif x==True:
    print("You won!!")
elif x==False:
    print("You Lost!!")


