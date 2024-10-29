# Vertical Slice PRD3 Shadows Over Suburbia
 Vertical Slice PRD3 of SOS 
 Play: 
 Full Project (including credits): https://github.com/mstrykul1336/Shadows-Over-Suburbia-Prototype-
 **10/28/24:**
 **What was done:**
- added a player's role to their death newspaper 
- added new UI at the top of the screen to display the day and night cycle number, a sun or moon, and the current timer.
- added a death journal, with a button in the top left corner. By clicking this button, you can type in your death journal and hit enter to write an entry. By clicking the button again you can close the journal and the entries stay saved.
- death journals will be displayed when a player dies
- added a fancy animation to the title screen looking over the town and at the town hall. eventually this will include villagers too.
- added a settings wheel that currently has the UI set up for volume settings, but there isn't sound in game so they don't have a purpose yet.
- added in all the controls into the control button in the menu.
- added using F1 to be able to see what roles and abilities are in the game while you are playing.
- added instructions in "how to play" in the title screen of the game. Added an extra button for alignments and their individual goals.
- changed the player list UI to a corkboard stained with blood to match the aesthetic. (text still moves around weird)
-when players die, they will be summoned back as ghosts in the town hall. Players shouldn't be included in voting or as players accessible in abilities. They shouldn't be able to access the inventory, night UI (such as their abilities), and journal.
    -   ghost players have a new model and have "ghost view" (currently just an image)
- It should display the player's role when they die in the newspaper, along with their name. (For me, it didn't always work. Sometimes it would say Mayor even if they weren't the mayor.)
- added in chat:
  - Global chat: you can see messages and send messages to other players. You will not be allowed to talk during night cycles (it will give a warning)
  - Local chat: This will give you feedback on your abilities or actions (such as you were attacked, you healed someone, etc).
  - Ghosts (or spectators) will not be allowed to chat.
  - added in game going back to main menu if you have only one player. 

 **To Do:**
 Changing players from disconnecting to spectating as ghosts (make sure in every loop that calls playerList that it also checks to make sure they aren’t dead.)  
Add in their roles into the newspaper if they die too (and eventually their profile picture image, so for now put a fake image there) 
Uncompress the game because I figured out GitHub (I had to compress textures for original upload, but I figured it out so now I can uncompress them again.) 
Make the real build for this week unplayable if there is only one player. (sends you back to main menu if you don't have enough players) 
Add in game direction in the how to play button, including:  
Explanation of each role and their goal depending on alignment 
Explanation of the controls 
Explanation of UI  
Explanation of voting mechanic  
Explanation of the shop and inventory functions  
Explanation on each ability 
Add in settings menu during the game where players can go back to read the guide from above in case they need to. 
Add a fancy animation to the title screen, showcasing the town.  
Add a death note/journal, where players can write in any information on each night and then this will display upon their death.  
On the playerlist UI, make it better. Fix the spacing and make sure the Mayor role is correctly marked on all player’s screens. Example: 
 image.png
Change the timer and day counter to the top in one neat UI box:  
Included here, add a night counter. Currently I only have a day counter UI.
 image.png
Maybe it is time for the good ol’ chat box to come back. If it ends up working out, change all of the player action logs to go into the local chat box (such as they were attacked, healed, took an action, etc).  
Make the UI better for abilities that give you information: 
Detective: Right now it just puts the log out in text, if the chat box idea does not work, I will fix it by making the UI prettier.  
 image.png
If chat ends up working, I will need a local chat (for actions only local player needs to see), global chat, and a dead player chat (optional).  
Backlog:   
Add in destructive and helpful versions of these abilities:   
Mayor: (currently has mayor's basement for helpful, but if destructive, you will be able to sacrifice the player to WiggleBlorp) 
Assistant (destructive would get brainwash, where you send an anonymous message to a player to invite them to the cult (destructive) side).  
Detective (destructive would get unlawful investigation, same investigation but you get the option to attack them, causing them to bleed for 1/4 hearts DOT for 3 nights) 
Medic (currently has heal, would need fake heal for destructive where it makes another player believe they were attacked and then healed) 
Everyone else gets the same ability no matter what side. 
Add in passives to two characters: Medic (immune to poison and bleed) & Clairvoyant (can't die at night, needs to be voted out). I need to make it so it doesn't give away their characters to any players though, just doesn't end up working if you attack them. 
