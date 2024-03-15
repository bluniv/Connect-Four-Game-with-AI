# Connect Four Game with AI

| Table of Contents: |
|--------------------|
| 1. Introduction |
| 2. Game Overview |
| 3. Gameplay Illustrations |
| 4. Implementation Details |
|           - 4.1 Game Mechanics |
|           - 4.2 AI Algorithm: Minimax with Alpha-Beta Pruning |
|           - 4.3 Integration of AI Algorithm |
| 5. How the AI Contributes to the Game |
| 6. Conclusion |
| 7. References |


1. Introduction:

The Connect Four game is a classic two-player strategy game where the objective is to be the first player to form a horizontal, vertical, or diagonal line of four of one's own discs. In this project, I have implemented a Connect Four game with an AI player using the minimax algorithm with alpha-beta pruning.

2. Game Overview:

Connect Four is played on a 6x7 grid, where players take turns dropping coloured discs into the columns. The discs fall to the lowest available space in the chosen column. The game ends when one player successfully forms a line of four discs in a row, column, or diagonal, or when the game board is full with no winner.


3. Gameplay Illustrations:                  




4. Implementation Details:

4.1 Game Mechanics:

- The game is implemented using Python and the pygame library for the graphical interface.
- The game board is represented as a 2D array using NumPy.
- Players take turns clicking on columns to drop their respective coloured discs.
- The game checks for win conditions after each player's move and ends the game if a player wins or if the board is full.

4.2 AI Algorithm: Minimax with Alpha-Beta Pruning:

- Minimax is a decision-making algorithm used for two-player games. It searches through the game tree to determine the best move for the current player, assuming that the opponent also plays optimally.
- Alpha-beta pruning is an optimization technique used with the minimax algorithm to reduce the number of nodes evaluated in the search tree.
- In our implementation, the minimax algorithm evaluates possible future game states by recursively exploring different moves up to a specified depth. It assigns scores to each potential move and selects the move with the highest score for the AI player and the lowest score for the opponent.
- Alpha-beta pruning helps to eliminate branches of the search tree that are guaranteed to be worse than previously examined branches, thereby reducing the number of nodes evaluated and improving the algorithm's efficiency.

4.3 Integration of AI Algorithm:

- The AI player uses the minimax algorithm with alpha-beta pruning to select its moves.
- It evaluates the possible future game states and selects the move that maximizes its chances of winning while minimizing the opponent's chances.
- The AI player considers various factors such as the current board position, potential future moves, and opponent's strategies to make informed decisions.

5. How the AI Contributes to the Game:

- The AI player adds a challenging opponent for the human player to compete against.
- It provides a dynamic and adaptive gameplay experience by making strategic decisions based on the current game state.
- The AI's ability to analyze potential future moves enhances the game's replay value and provides opportunities for players to improve their skills.

6. Conclusion:

In conclusion, the Connect Four game with an AI player demonstrates the integration of an AI algorithm to enhance the gameplay experience. The minimax algorithm with alpha-beta pruning enables the AI player to make intelligent decisions, adding depth and challenge to the game. Overall, this project showcases the application of AI in game development and its impact on player engagement and enjoyment.

7. References:

- Russell, S. J., & Norvig, P. (2016). Artificial Intelligence: A Modern Approach (3rd ed.). Pearson.
- Pygame Documentation: https://www.pygame.org/docs/
- NumPy Documentation: https://numpy.org/doc/
