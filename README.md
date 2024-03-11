# The-100-game-
That's code for game 

#welcome message & initial value of Sum
print("welcome to our game")
print("the winner who reaches 100")
print("The sum is 0 now")

Sum=0
lst=[1,2,3,4,5,6,7,8,9,10]

#the start of the game
while(True):
    
    while(True):  
       #first player and his process
       plyr_1=int(input("player1,please choose a number from 1-10>>"))
       if(plyr_1 in lst):
         
          if(Sum==(100-plyr_1)):
             print("player 1 is the winner")
             exit()
          if(Sum<100 and plyr_1 <=(100-Sum)):
             Sum+=plyr_1
             print("the sum is ",Sum," now")
             break
          if((Sum<100 and plyr_1 >=(100-Sum))or (Sum>100)):
             print("Enter a smaller number>>")
             continue
        
       else:
          print("enter a valid number from 1-10>>")
          continue
        
    while(True):  
       #second player and his process
       plyr_2=int(input("player2,please choose a number from 1-10>>"))
       if(plyr_2 in lst):
         
          if(Sum==(100-plyr_2)):
             print("player 2 is the winner")
             exit()
          if(Sum<100 and plyr_2 <=(100-Sum)):
             Sum+=plyr_2
             print(" the Sum is ",Sum," now")
             break
          if((Sum<100 and plyr_2 >=(100-Sum))or (Sum>100)):
             print("Enter a smaller number>>")
             continue
        
       else:
          print("enter a valid number from 1-10>>")
          continue
