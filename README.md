# Conan-Clue
A pippi game that tries to be like clue but in conan.

# Disclaimer.
This is a work in progress. As of right now only one murderer, murder weapon, and murder room can be selected. The Jokes are very meta for the Chains server, as this is just a proof of concept. The full release will be more PG 13 so any server can use it.

# Setup

1) Add scripts to each of the thespians in the mansions. There are four suspects that should be in various rooms. (Already labeled) The suspects only have limited appearance requirements. Alice is female and larger than the other suspects. The barrier is male and should be dressed in colors similar to Alice. Salerno is male. Demure is female. Jason the dead body is male and should be frozen in a laying animation in the kitchen. A male guard should be outside the door to the kitchen.  

The rest of the thespians and look any way you want them to. The make guess, rewards (cop 1 and cop 2), and butler (event starter) are all thespians players will need to interact with. The Admin reset and Admin Check Vars thespians should ignore all non admin players. Admin reset will allow Admins to play again or start over. Check Var is for troubleshooting bugs. As of right now players can only play once. Later the event starter thespians will reset all char vars when giving out the quest, so non admins can play again.

2) An egress door should be placed on the kitchen door. There are few ways for players to figure out the passcode for the door and there is a secret way into the room if players find it. No other placeables are required at this time. (Remove the pippi note after the egress door has been added)

3) To start the event an admin must speak with the event starter thespian. Even though only one option is available you must still use the dialogs. 
A) "I want to setup or change..." Only acceptable values right now are "A horse dildo, BallRoom, Alice" 
B) Next set the egress code. It will pick a random code. Make sure you set the passcode for the egress to match the value from the dialog.
C) I am ready to start the event. 
D) You can pick I am ready to play to play along (or test) as well.

4) Players can lock in their guesses at any time. Once they make a guess, they cannot change it. Once they have voted they can find out if they won or not.  Admins can end the event two ways. Speaking with Event Starter they can 
A) Stop the event, but leave guessing and reward npcs active. This way, if anyone started the quest, but had to leave, crash, or whatever they can still come back and make guesses but none of the other thespians will speak to them. 
B) Stop the event and disable all thespians. (I plan to make this more customizable later)

5) The only scripting changes that must be done manually are setting cool down for quests, the reward, and the option to have the killer (Alice) teleport players outside of the event instead of killing them on the spot. Players still fail the quest if the killer or guard kills them, but having dead bodies lying on the ground next to Alice may give things away too much.
