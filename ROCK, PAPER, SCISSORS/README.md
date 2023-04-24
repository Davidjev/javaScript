# README File for Rock-Paper-Scissors Game

This is a simple implementation of a Rock-Paper-Scissors game using JavaScript. The game allows a user to play against the computer and determine the winner based on the choices made.

### Usage

To play the game, simply load the HTML file in a web browser and click on the "Start Game" button. The game will prompt the user to make a choice between Rock, Paper, or Scissors. The computer will then randomly select a choice, and the winner will be determined based on the rules of the game.  

If the user enters an invalid choice, the game will choose Rock as the default choice for the user.  

### Code Structure

The code consists of the following components:

- startGameBtn: An HTML button element that triggers the start of the game.  
- ROCK, PAPER, SCISSORS: Constant variables that represent the three choices available in the game.  
- DEFAULT_USER_CHOICE: A constant variable that represents the default choice (Rock) for the user.  
- RESULT_DRAW, RESULT_PLAYER_WINS, RESULT_COMPUTER_WINS: Constant variables that represent the possible outcomes of the game.  
- gameIsRunning: A boolean variable that determines whether the game is currently running.  
- getPlayerChoice(): A function that prompts the user for their choice and returns it.  
- getComputerChoice(): A function that generates a random choice for the computer.  
- getWinner(cChoice, pChoice = DEFAULT_USER_CHOICE): A function that compares the computer's choice with the player's choice and returns the winner.  
- startGameBtn.addEventListener(): An event listener that starts the game when the "Start Game" button is clicked.  
- 
