# TIC ⋆ TAC ⋆ VOTE
A partriotic twist on the classic game

## How the Game is Played

1. The user/player selects whether they want to play a two-player or one-player game. The default selection is a two-player game, and in that version, the user plays alongside another player, using the same mouse. In a one-player game, the user plays against the computer.

2. **Two-Player Game**  
The first player is a member of the X Party, so they place an "X" on any empty square on the gameboard. They do this by simply clicking their selection. The second player is a member of the O Party, and they too click on the empty square of their choice.

3. **One-Player Game**  
The user is a member of the X Party, so they place an "X" on any empty square on the gameboard. They do this by simply clicking their selection. After a few seconds, the computer—filling the role of the second player—automatically makes its selection, marking one of the empty squares with an "O".

4. Play continues back and forth until a player has claimed three squares in a row for their party, resulting in a win. The game instantly ends, and the winning player's score, or total wins, increases by one. 

5. If every square is claimed and neither player has three in a row, the game ends in a tie. In this case, neither player's score increases.

6. The user starts a new game and resets the gameboard by clicking "Play Again".

7. **NOTE:** Starting a new game does not reset the players' scores. However, changing from a two-player game to a one-player game, and vice versa, DOES reset the scores.


## Functions

This is a guide to the functions found in `app.js`.

| Function | What it Does |
| ----------- | ----------- |
| `changeNumPlayers` | Changes the game mode from two-player to one-player, and vice versa; also resets the players' scores |
| `handleClick` | Determines what to do based on several factors: which square is clicked, whose turn it is and whether it's a one-player or two-player game |
| `updateGameboard` | Updates the appearance of the gameboard with the current player's choice and the next prompt |
| `handleClickOnePlayer` | Handles the user's moves in a one-player game |
| `computerMoves` | Handles the computer's moves in a one-player game |
| `checkforWin` | Compares the current gameboard against a list of possible scenarios, to determine if a player has won; runs after every move |
| `compareValues` | Handles the actual comparisons in `checkforWin` |
| `displayWinMsg` | Updates the appearance of the gameboard when a win is determined |
| `checkForTie` | Determines whether the game has ended in a tie; runs after every move |
| `displayTieMsg` | Updates the appearance of the gameboard when a tie is determined |
| `displayPlayAgain` | Adds a "Play Again" link below the gameboard when a game ends |
| `resetGameboard` | Clears the gameboard for another game |


## Installation

To install a local copy of the game's build files, follow the steps below.

1. Fork a copy of the game's repository [here.](https://github.com/delayedaa/tic-tac-toe.git)

2. Clone the copy to your local computer by typing the following code in your terminal:
```
git clone https://github.com/delayedaa/tic-tac-toe.git
```

3. Navigate to the cloned directory and open `index.html` in your browser by typing the following code in your terminal:
```
open index.html
```

## Notes

- At the bottom of `app.js` is some code that has been commented out. Please disregard it for the moment; work is currently being done on a potential upgrade to the computer's difficulty level when playing in one-player mode.