#KenTacToe
* Author(s): Kenshin Himura *(Sudarsan Balaji)*
* License: *GNU GPL v3* (see COPYING.texi)
* Application Version: 2.7
* ReadMe Version: 1.9

##Description
A basic Tic Tac Toe (TTT) game engine able to present an AI capable of playing Tic Tac Toe with humans on boards upto 11x11 boxes.
The entire game engine has been completed. Game has grid and players and is made up of moves and searches.
Game has minimax search with alpha-beta pruning and an evaluation function which has the capability to work in any grid size.
*See __Misc__ section of Updates for further information.*

##Features
* Fast play even on large boards.
* Automatic Optimum Search Depth calculation *(from free space for Java VM)*.
* Mini-Max search with Alpha-Beta Pruning.
* Player vs. Player / AI.
* Play on upto 11x11 grids.
* Robust Evaluation Function.
* Ultra-Strong AI.
* Close-to-real-world in-game representation of the game, thanks to maximally implemented OOPS concept *(suggestions for improvement welcome)*.

##Updates

###Version 2.7
* Fixed issue with Play Again.

###Version 2.6
* Further optimization
* Faster Play when playing on larger boards by cutting down on search depth *(also optimization :D)*.
* Removed searchDepth debug messages *(which I accidentally left out in version 2.5!)*.

###Version 2.5
* Bug fixes for issues caused by improper optimization.
* Fixed memory leak.
* Fixed searchDepth changing from lower to higher after optimization.

###Version 2.4
* Included classmexer.jar
* Included classmexer readme.txt
* Now automatically selects maximum search depth depending upon available free memory *(thanks to classmexer)*.

###Version 2.3
* Included application name, version and author definitions.
* Added option to play again.
* Minor changes in play() function of Game class.
* Main not calling init() anymore, only play().

###Version 2.2
* Major overhaul of a lot of code.
* Tremendous amount of optimization.
* Changed all possible integers to byte, thereby reducing memory footprint. *(Even 11x11 box has only 121 boxes, less than 8-bit byte)*

###Version 2.1
* Added choice for users to play against AI or against another user(human).
* Rewrote Main to allow for this choice.
* Wrote another Game constructor to implement this choice.
* Added a Win-32 exe to run on java-enabled Windows PCs.

###Version 2.0
* Removed debug Messages.
* Added exported Executable-JAR file.
* All aims of project achieved. Hopefully no more TODO's until requests from others. :)

###Version 1.9
* Various optimizations.
* Restructured various functions and their definitions.
* Minor stability updates.
* Minor bugfixes.

###Version 1.8
* Updated Evaluation Function.
* Fixed the buggy AI (at last!).
* Minor bug fixes.

###Version 1.7
* Now game asks for search depth, to implement fixed search depth in cases where grid size varies.
* Invalid search depths are corrected with default values.
* Wrote new constructors and callers to implement search depth functionality utilization.
* Corrected evaluation function, now symmetric boards (same chance for winning for both X and O) give an evaluation score of "0.0".
* AI still buggy a bit, have to investigate.

###Version 1.6
* Now game asks user for choice between playing as X or as O. AI works for any one.
* Now game asks user to choose grid size, not just 3x3 games anymore.
* Updated evaluation function and search function to work with all board sizes, and AI can play both as X and O.
* Minor bugfixes in search function.
* Minor corrections in evaluation and search code.
* Rewritten large volumes of code to implement these choice based decisions in Game, Player, Table, Search and Main classes.
* AI still buggy a bit, because evaluation function remains unchanged in core functionality from  version 1.5.

###Version 1.5
* Updated evaluation function.
* Corrected major bugs in evaluation helper functions.
* Rewritten lots of evaluation-helping code.
* Fixed a few memory leaks.
* Out of 6 features for evaluation, 2 return non-zero values even on symmetric boards. Solution being worked upon.
* Modified Alpha-Beta Search function.

###Version 1.4
* Evaluation function made more robust.
* Added extra features to evaluate.
* Minor bugs removed.
* AI still buggy, have to fine-tune the evaluation.

###Version 1.3
* Minor bug and stability updates.
* Evaluation function updated to work with any grid size (not restricted to 3x3 box any more).
* AI almost still the same, with little to no modification.
* Scoring system has been updated to double type instead of float to allow for more range of numbers to be used.

###Version 1.2
* Minimax with Alpha-Beta Pruning implemented, though a bit buggy.
* More robust evaluation function for 3x3 boxes.

###Version 1.1
* NegaMax search implemented.

###Version 1.0
* Game fully functional now. Rules are followed, AI picks move (though not the best!). Game ends when win conditions are met. AI to be implemented with minimax or something soon.
* Table.java now with full commentary.
* All java files are now with full @javadoc commentary. Enjoy learning!

###Misc
* Efforts have taken to make the source code readable by adding comments wherever absolutely required.
* Additional commentary will be provided if required (or on request).
* An important aim of this project is to make legible and understandable well-commented code, but that doesn't mean every line of code has been commented. If additional assistance is required by anyone reading the code, please do post a message asking for such assistance as can be provided (basically, more comments in the source code, that's all!).
* ReadMe updated to reflect version changes chronologially now.
* With version 2.0, the main aim of the project has been accomplished. Further optimization suggestions are welcome.
* Description updated stating 11x11 boxes instead of the original vision of 255x255 boxes, due to the limitations placed on the double data type used to calculate the score. To provide for more boxes, either the evaulation function should be modified or something else has to be done. Mmmm, not sure. Let's leave it as such. Isn't playing on 11x11 boxes enough? :D

##Visions
* Optimizations of any sort on the existing code.
