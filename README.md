# Udacity_TicTacToe

This is the final project for the [Udacity Java Programming Basics class](https://www.udacity.com/course/java-programming-basics--ud282). Rather than utilizing IntelliJ this repo is the TicTacToe project ported to VSCode. 

### Table of Contents

[Installation](#installation)

[TicTacToe Problem](#tictactoe-problem)

[Debugging](#debugging)

## Installation
1. Install VSCode (Skip this step if VSCode is installed)
Recommend you install the WPILib VSCode as it is what we will use for FRC, but you do not have to.
- Install [.Net Framework 4.6.2](http://go.microsoft.com/fwlink/?linkid=780600)
- Download WPILib VSCode [64-bit.zip](https://github.com/wpilibsuite/allwpilib/releases/download/v2019.4.1/WPILibInstaller_Windows64-2019.4.1.zip) - see more information about installtion [https://github.com/wpilibsuite/allwpilib/releases](https://github.com/wpilibsuite/allwpilib/releases)

2. Install git (Skip if git is installed) [https://git-scm.com/download/win](https://git-scm.com/download/win)
*DO NOT INSTALL GIT CREDENTIAL MANAGER* unless it's your personal computer, it'll ask in one of the steps during installation.

3. Clone this repository or download the .zip code

4. Open VSCode. Then File -> Open Folder and open the Udacity_TicTacToe folder.

5. Press Ctrl + Shift + B, if the latest gradle version is not installed it will, and then it should open up a new window which is the TicTacToe game. 

## TicTacToe Problem
### Code design
The source code includes 2 main Java files, Game.java and GameUI.java.

1. Game.java is where all the game logic code exists.
2. GameUI.java is where all the user interface code exists. You can take a look at GameUI.java if you like, but it is not necessary to change any code there to complete the project.

Your job is to implement the checkGameWinner() function in the Game.java file.

String checkGameWinner(char [][] grid) has a 2D char array as an input representing the game grid (see below for details) and it returns a String message indicating which player has won (X wins , O wins, Tie, or None if the game hasn't ended yet)

The Grid is represented as a 2D array of characters, indexed as follows:
top-left is 0,0
bottom-right is 2,2

### Requirements
In checkGameWinner() you should access those cells in the 2D array to find out if X or O has won the game by checking if there’s 3 of the same kind in a row either horizontally, vertically or diagonally!

1. If you detect a winner, set the variable result to either “X wins” or “O wins” depending on the player who won.
2. If the game ends as a tie, set result to “Tie.”
3. If the game has not ended yet set result to “None.”

Then make sure the function returns that variable result at the end (you can also return the string literal directly as you detect a winner or tie).

## Debugging
As you develop the code for the problem above you might find that you want to investigate what is happening with a variable or in a certain function, that's where debugging comes in. See Udacity's lecture about debugging to learn more. 

Since we are using VSCode you'll want to refer to [VSCode Java Debugging guide](https://code.visualstudio.com/docs/java/java-debugging)

