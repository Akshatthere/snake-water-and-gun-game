# snake-water-and-gun-game
#snake and water gun
import random
def check(comp,user):
 if comp ==user:
    return 0
 if(comp==0 and user==1):
    return -1
    if(comp==1 and user==2):
     return -1
     if(comp==2 and user==2):
      return -1
      return 1
comp = random.randint(0,2)
user=int(input("0 for sanke, 1 for water and 2 for gun "))
score = check(comp,user)
print("your choice :",user)
print("computer choice :",comp)
if(score == 0):
  print("nice its a Tie")
elif (score == -1):
  print("uffo you loose")
else:
 print("hurrah you won ")
