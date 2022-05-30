# Treasure-Island
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 

#https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Treasure%20Island%20Conditional.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1oDe4ehjWZipYRsVfeAx2HyB7LCQ8_Fvi%26export%3Ddownload

#Write your code below this line 👇


# Direction Variables
a = "left"
b = "right"

dir_a = a.lower()
dir_b = b.lower()

#Action Variables
c = "swim"
d = "wait"

act_c = c.lower()
act_d = d.lower()

#Door Choice Variables
e = "red"
f = "blue"
g = "yellow"

choice_e = e.lower()
choice_f = f.lower()
choice_g = g.lower()

#Game Execution

decision_1 = input(f"You're at a crossroad in a dense dark forest. Which way would you like to go {dir_a} or {dir_b}?")


if decision_1 == "left":
  decision_2 = input(f"You are now at a lake and can either swim or wait for a boat. Would you like to {act_c} or {act_d}?")  
  if decision_2  == "wait":
    decision_3 = input(f"You are in a mansion with many doors. One is {choice_e} , one is {choice_f}, and the other is {choice_g}. Would you like to go through the red door, blue door, or yellow door?")
    if decision_3 == "red":
      print("You have entered a firey room. Game Over")
    elif decision_3 == "blue":
      print("You were eaten by beasts. Game Over.")
    elif decision_3 == "yellow":
      print("You have discovered the treasure. You Win.")
    else:
      print("You've chosen a door that is not a choice. Try again.")
  else:
    print("You were attacked by a crocodile. Game Over.")  
else:
  print("You fell into a hole. Game Over.")
