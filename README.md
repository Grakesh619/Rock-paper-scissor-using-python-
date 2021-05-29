# Rock-paper-scissor-using-python-
Let's play rock paper scissor 


import random
hum_board =0
com_board =0

tie=0
while(True):
  
  
  hum_choice = input("enter your choice : \n1.Rock\n2.paper\n3.scissor\n")
  print("Human choice is :", hum_choice)
  com_lst = ["rock","paper","scissor"]
  com_gen=random.choice(com_lst)
  print("computer generated :",com_gen)
  

  if hum_choice=="paper" and com_gen=="paper" or hum_choice=="rock" and com_gen=="rock" or hum_choice=="scissor" and com_gen=="scissor":
    tie = tie + 1

  elif hum_choice=="rock" and com_gen=="paper":
    com_board=com_board+1

  elif hum_choice=="rock" and com_gen=="scissor":
    hum_board=hum_board+1

  elif hum_choice=="paper" and com_gen=="rock":
    hum_board=hum_board+1

  elif hum_choice=="paper" and com_gen=="scissor":
    com_board=com_board+1

  elif hum_choice=="scissor" and com_gen=="rock":
    com_board=com_board+1

  elif hum_choice=="scissor" and com_gen=="paper":
    hum_board=hum_board+1
  
  rep =input("Do you u want to continue(Yes/NO) :")
  if rep == "Yes":
   continue
  else:
    break
