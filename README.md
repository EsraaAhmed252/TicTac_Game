# TicTac_Game

https://github.com/EsraaAhmed252/TicTac_Game/assets/99142254/3fb4fa7f-5642-46a9-ae7e-cb7ee4546c60

implementation of the game Tic-Tac-Toe with a computer player using the minimax algorithm for making decisions. 
Here's an overview of the algorithm and a breakdown of the code:

### Algorithm: Minimax

The minimax algorithm is a decision-making algorithm used in two-player games with perfect information, like Tic-Tac-Toe. It's used to determine the optimal move for the player given the current state of the game. The algorithm considers all possible moves and outcomes, assigning scores to each move based on the outcome. It aims to minimize the potential loss (for the opponent) while maximizing its own potential gain.

In the context of Tic-Tac-Toe, the algorithm recursively explores all possible future game states and assigns scores to them, then selects the move with the highest score when it's the computer's turn, and the move with the lowest score when it's the opponent's (human's) turn. The algorithm assumes both players play optimally.

### Code Breakdown:

1. The code begins by defining constants for player types and move symbols.
2. The `showBoard` function displays the Tic-Tac-Toe board.
3. `showInstructions` displays instructions for the game.
4. `initialise` initializes the game board with empty cells.
5. `declareWinner` function prints out the winner of the game.
6. `rowCrossed`, `columnCrossed`, and `diagonalCrossed` functions check if a player has won in a row, column, or diagonal respectively.
7. The `gameOver` function checks if the game is over by checking if any player has won or if the board is full.
8. `minimax` function is the core of the algorithm. It recursively evaluates all possible moves, assigning scores based on the outcome of the game. It returns -1 if the computer wins, +1 if the human wins, and 0 for a draw.
9. `bestMove` function calculates the best move for the computer using the minimax algorithm. It considers all possible moves, evaluates their scores, and selects the move with the highest score.
10. The `playTicTacToe` function is the main game loop. It alternates between the computer and human turns, making moves and updating the board accordingly.
11. The `main` function initializes the game and allows the player to choose whether to play as the first player or second player (against the computer). It keeps asking if the player wants to play again after each game.
