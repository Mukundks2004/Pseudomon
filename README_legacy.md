README
PSEUDOMON BY MKS

Haha excuse my absolute failure at a readme i've only ever done a few :P

#Pseudomon
Pseudomon is a project for a game resmbling the start of pokemon red.

#Running
Run the .py file from the folder (not quick access) and wait for the game to load.
This will take up to a minute depending on PC RAM and background processes running
The game is ready to be played once the title screen has loaded and the music has started
If the music starts but the title screen is black, select a small portion of the screen and hit the down key.
If the full screen loads inside a small box, resize the box to fit the screen manually (don't use the fullscreen button). The screen should go black. Once you are SURE it is big enough, press z and the game will commence with the new resized screen.
If all else fails, close the window and load again.


#Keys
When in intro/through dialogue:
    Z key for pressing enter and progressing through speech
When in game:
    Arrow keys for navigation
    Z key to talk to people or read signs
    X key to save gamestate (pokemon, location, xp and inventory)
    C key to load gamestate (pokemon, location, xp and inventory)
    V key to read inventory
When in battle:
    Up and down key to navigate attacks
    Z key to read dialogue and to confirm an attack
    X key to throw a pokeball
    C key to use a potion
    

#How to play
The game consists of 3 stages
Stage 1:
    Scroll through the starting dialogue to read the lore
Stage 2:
    Play the game, move through the maps and capture pokemon
Stage 3:
    Battle Blue's Raticate and win, ending the game
    
#Moving
Move using the arrow keys
The framerate is ~1 fps. This is editable if the user's PC has good processing capabilities. See #Framerate
The user can only move one space per frame.
Keypresses are loaded into the keypress log.
This means that spamming "forwards" 10 times will set the user up to move 
10 spaces sideways over the next 10 seconds.
THE USER MUST USE THEIR KEYPRESSES WISELY. NEVER SPAM.
The user cannot walk off the map or into walls. The user can try.
Some rails are one-way and can be jumped over downwards but no passed through upwards.


#Pokemon
Pokemon are the user's arsenal. A pokemon is a weapon in the form of a pet
that is used to fight other NPC's pets. They also fight wild pets. Pokemon
have a total amount of hit points that they can take before fainting. If they faint
they must be healed at an official healing centre.
When attacking, pokemon have a predefined list that they can choose from.
Each attack will either damage the opposing pokemon, weaken the opponent
or buff themselves. Some pokemon are stronger than others.
Pokemon have elements associated with them. A weaker pokemon may defeat a stronger
one by being of a superior (or advantageous at least) type. Specific attacks
are not associated with types.
Pokemon have a level associated with them as well. Higher levelled-pokemon are stronger.
Pokemon do not evolve into other pokemon if their levels reach any threshold.

#Random Encounters
When walking in tall grass there is a chance of the user battling a random wild pokemon

#Battle
The user can either battle pokemon in random encounters or can fight Blue.
Random encounters will be selected from a list of pokemon. The user is more likely to 
battle some pokemon than others. First, the user may select an attack out of 2 options
(themselves selected from the pokemon's attack). An attack will either be offensive
or tactical. Offensive attacks deal damage. Tactical attacks have a 50/50 chance
of either increasing the user's attack power or decreasing that of the wild pokemon's.
If the wild pokemon has not fainted (which occurs if they reach 0 hp), they will then attack.
If the player's pokemon has not fainted, they may attack. Optionally, the player
may choose to use an item on their turn. The opponent will never use items. See #Items.
When either pokemon faints, the other wins. The user cannot send more than one pokemon to battle.
If all the user's pokemon faint, they will not be allowed to battle until health has been restored.
See #Services.

Note- attacks have a low chance of missing. Any buffs or debuffs acted
on the player during the attack are semi-permanent. See #Services. 

#Items
Players may collect two types of items, which can be used during battle.
Pokeballs can be thrown on a user's turn. Not having pokeballs hile attempting to use one
will result in the user losing their turn. Pokeballs may fail or succeed to catch ANY pokemon
if the pokemon's hp is lower than a certain threshold.
Potions can be applied to player's pokemon to increase their hp by 100
irrespective of their maximum hp. not having potions while attempting to use one
will result in the user losing their turn.

The user has a random chance of stumbling upon either pokeballs or potions anywhere
while moving in the game. These items can be viewed in the inventory. See #Keys.

These items may also be purchased in the shop. See #Services.

#Services
Services come in the form of one of two kinds. The pokecentre is 
in Viridian City and will restore all the user's pokemon to their full hp 
with no charge. They also reset buffs. If all the user's pokemon faint, the user will
be taken to the pokecentre and the user's health will be healed.

The pokemart is also in Viridian City. Potions and pokeballs can be purchased
for xp. See #Xp

#Xp 
Xp is the currency of the game
The user can win xp by battling pokemon and winning, in which case they will be
given the same amount of xp as the total health of the losing pokemon.

#Framerate 
Located in the Gamespeed variable on line 7 of the code.
The user may lower this for a better playing experience if they have a good pc
that can load frames quickly. 
This may require tweaking, as if the framerate is set too low,
majority of the time spent waiting will be waiting for the 
frame to render rather than waiting in between frames as intended.
TO REITERATE, CHANGING THE FRAMERATE DOES NOT DECREASE PRINT SPEED!
IT DECREASES THE TIME SPENT WAITING IN BETWEEN FRAME PRINTS
THAT WERE INTENTIONALLY ADDED TO BALANCE THE FEEL OF THE GAME.

#Notes
3 pseudocodes are attached. The first is using the requested notation but that is not designed for this kind of project, and as such is ineffective.
The second is a better version that follows an adjusted version of the widely used AQA code. 
The third contains no formatting but is the easiest to follow- it is literally just english, consisting of edited versions of the comments.

The pdf contains a poorly formatted version of the flowchart. The __main__ is the main routine, all separate flowcharts are the functions. The __str__ is the output print (string) function.