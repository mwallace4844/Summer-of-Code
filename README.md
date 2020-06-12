# Summer-of-Code
## How to run my code
 Run main.py. Arcade must be installed. The most up-tp-date version is in the "06.11.20" folder. 
## Motivation
 At Hamilton, the ice cream machine is Commons is very adored. I wanted to create a game that involved a little bit of strategy (what order to eat the ice cream and pick up the bowls in). 
 ## Description
 In this game you are Alexander Hamilton! Use the arrow keys to move around. When touching an ice cream, you can press "E" to eat it. You can press "P" to pick up a bowl. You must eat the ice cream before picking up a bowl. You cannot eat ice cream if you are carrying a bowl. If so, you lose. You can pick up as many bowls as you want. You can press "D" to drop a bowl. The goal of the game is to eat all the ice cream and to place all the bowls on the conveyor belt as quickly as possible.
 ##Keys
 **Arrows** - moves Alex
 **E** - Alex eats the ice cream
 **P** - ALex picks up a bowl
 **D** - Alex drops a bowl
 **SPACE** - begin the game and play again
  ##Challenges/Lessons
 Determining how to move the bowls in sync with ALex was challenging. Check_for_collision_with_list would return the bowls that Alex was already carrying. If this occured, the bowls that were picked up first would move the fastest. I fixed this by not adding a sprite returned from the check_for_collision_with_list function to self.carrying if it was already in the list. 
 Another issue I encountered was making it so you had to eat the ice cream before picking up the bowl. This was difficult because I had to link three variables together: the bowl sprite, the ice cream sprite, and a boolean of if the ice cream was eaten or not. A list would not be sufficient because the order one eats the ice cream in is not necessarily the same order that the sprites were created in. I fixed this problem by creating two dictionaires. 
 ##Future Steps
Adding in obstacles that the player must move around. 
