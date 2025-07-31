# Strands Remake: James Rosenberger
This is a modified version of a project I completed for my CMSC 14200 course which features only those implemenations (GUI and Game Logic) I was responsible for creating. The files corresponding to these components are src/gui.py, src/strands.py (the most recent logic), and src/fakes.py (an earlier logic no longer used). Consider that the other ui/art and test files remain not as contributions of my own, but rather as supplements from project teammates that I could use should I choose to expand the project later. Below, I will describe how you can play this game yourself.

## How to Play:
Before anything, clone all files locally and ensure all requirements are met. At its most basic level, this game can be run with a random background board by running python3 src/gui.py from the root of your local directory. However, I've added a number of optional command-line parameters to be included after python3 src/gui.py that can add make your game expeirence more dynamic and interesting. Below they are explained. Note that, just like the actual game, you can click adjacent letters on the board to build a strand, double click the last letter in a any strand to submit it, and click in non adjacent letters or press "esc" to reset the strand. Hints are collected by submitting strands that are non-theme dictionary words of at least length three, and you use a hint when available by pressing "h". For the hint word under consideration, the first hint will reveal using green circles the location of all letters that make up the word in question, while the second while use red circles to reveal the starting and ending letter of said strand. I hope you enjoy the game!

## Command-Line Parameters

--show which is a flag to indicate that the UI should immediately show the answers instead of having the user play the game. This corresponds to the game having two modes, Show and Play, the former being called via this parameter.

-g GAME / --game GAME to specify which game to load; the corresponding file is boards/GAME.txt. If this parameter is not provided, the UI will select a game at random.

-h HINT_THRESHOLD / --hint HINT_THRESHOLD to specify the hint threshold. The default is 3.

-a FRAME / --art FRAME to specify which kind of frame to display. Possible frames include cat0, cat2, cat3, and cat4. If this --art parameter is not provided, the UI will select cat3 as the default. These frames we all designed by a partner in the project.

For example, it is be possible to run the GUI like this:

python3 src/gui.py: This will start a randomly selected Strands game in the GUI, with a hint threshold of 3 and the cat3 frame.

python3 src/gui.py --show -g cs-142: This will launch the Strands GUI, displaying the solution to the “CS 142” game file.

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
Play or Show mode command-line arguments. Doing so will create
a new GAME.with-words.txt file in the assets/ directory from the original
file specified by -g game in the command-line. This newly created file, if
made, is NOT used by the Game Logic, as this addition was optional. Enjoy!


