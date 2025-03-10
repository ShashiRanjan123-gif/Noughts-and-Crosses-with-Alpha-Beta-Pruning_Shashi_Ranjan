# Noughts-and-Crosses-with-Alpha-Beta-Pruning_Shashi_Ranjan
Noughts and Crosses (Tic-Tac-Toe) with Alpha-Beta Pruning
Project Overview
This repository contains an implementation of the Noughts and Crosses (also known as Tic-Tac-Toe) game with an AI opponent that uses Alpha-Beta Pruning to optimize decision-making. The AI uses the Minimax algorithm enhanced by Alpha-Beta Pruning to determine the best moves and challenge a human player.

Game Features:
AI (X) vs Human (O): The AI plays as "X", and the human plays as "O".
Alpha-Beta Pruning: Speeds up decision-making by pruning branches of the game tree.
Game Flow: Alternates turns between the AI and the player until there's a winner or a draw.
Table of Contents
Installation
How the Game Works
Code Explanation
Game Screenshots
Contributing
License
Installation
Prerequisites:
Python 3.x (Recommended version: 3.7+)
Steps to Run the Game:
Clone this repository:

bash
Copy
git clone https://github.com/yourusername/tic-tac-toe-alpha-beta-pruning.git
Navigate to the project directory:

bash
Copy
cd tic-tac-toe-alpha-beta-pruning
Run the Python script:

bash
Copy
python tic_tac_toe.py
No additional libraries are required, as the game relies solely on Python's built-in functionality.

How the Game Works
Game Representation:

The game board is a 1D array with 9 positions.
0 = Empty spot, 1 = AI's move (X), -1 = Player's move (O).
Minimax Algorithm:

The AI evaluates all possible moves, assuming both the player and the AI play optimally. The Alpha-Beta Pruning technique optimizes this process by pruning unnecessary branches of the decision tree.
Player's Input:

The player enters a number between 0 to 8, which corresponds to an empty position on the board.
AI's Move:

The AI calculates the best move based on the current board configuration using the Alpha-Beta Pruning method.
Winning Conditions:

The game checks for a winner after every move. A player wins by aligning three marks horizontally, vertically, or diagonally.
Code Explanation
The game logic is implemented in Python using the following key functions:

check_winner():

Checks if a player has won by looking at all possible winning combinations.
is_game_over():

Determines if the game is over by checking if there's a winner or if all positions are filled.
alpha_beta():

Implements the Alpha-Beta Pruning algorithm. This function recursively evaluates the game tree, pruning branches that don't affect the final outcome, significantly speeding up decision-making.
best_move():

Finds the best move for the AI by evaluating all possible moves using the alpha_beta() function.
print_board():

Displays the current state of the board after each move.
play_game():

Manages the game flow, alternating between the AI and the human player.
Game Screenshots
1. AI's Move

2. Player's Move

3. Game Over (AI Wins)

Contributing
We welcome contributions to improve the functionality and performance of this project. If you'd like to contribute, please follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature-name).
Make your changes.
Commit your changes (git commit -am 'Add new feature').
Push to the branch (git push origin feature-name).
Open a Pull Request.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Minimax Algorithm: A decision-making algorithm used in game theory, where the AI evaluates all possible outcomes to make the best move.
Alpha-Beta Pruning: An optimization technique that reduces the number of nodes evaluated in the decision tree, improving the AI's performance.
Tic-Tac-Toe: A classic game used to demonstrate the power of AI algorithms.
Important Notes:
The game is designed to run in a terminal or command-line interface (CLI). It currently doesn't have a GUI.
You can modify the AI to play against itself or develop a graphical user interface for better interaction.
How to Add Images in GitHub README
Place your screenshots or images in a folder (e.g., images/).
Reference the images with relative paths in the Markdown (e.g., ![AI's Move](images/ai-move.png)).
This README is ready for you to add to your GitHub project. You can replace placeholder sections (like path-to-your-image) with the actual file paths or URLs to your images if you want to display screenshots of the game in action.
