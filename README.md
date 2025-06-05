# Strands Remake: James Rosenberger
This is a modified version of a project I completed for my CMSC 14200 course which features only those implemenations (GUI and Game Logic) I was responsible for creating. Below, I will describe how you can play this game yourself.

## Enhancements:
As a part of the project, I was required to contribute some enhancements to the original functioning of the game. Below are two that I created with explanations on how to run them locally.

### GUI-SOUND:
For testing the game with sounds, use the optional
command-line parameter --sounds in addition to all the other normal
Play or Show mode command-line arguments. Note the Play mode sounds
are more extensive. I've added sounds
from https://kenney.nl/assets/category:Audio?search=&sort=update
for starting the game, quitting/exiting, clicking, clearing by
hitting escape, submitting a too short, non-dictionary, or repeated word,
and for both submitting a new dictionary and new
strand word. Enjoy!

### DICTIONARY-WORDS:
For testing this functionality, use the optional
command-line parameter --words in addition to all the other normal
PLay or Show mode command-line arguments. Doing so will create
a new GAME.with-words.txt file in the assets/ directory from the original
file specified by -g game in the command-line. This newly created file, if
made, is NOT used by the Game Logic, as this addition was optional. Enjoy!


