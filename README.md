# Tic Tac Toe Game

## Project Overview

This project is a web-based **Tic Tac Toe** game built using HTML, CSS, and JavaScript. It allows a user to play against an AI, which uses the Minimax algorithm to make optimal moves. The game follows the traditional Tic Tac Toe rules, where two players (X and O) take turns marking a 3x3 grid. The first player to get three of their marks in a horizontal, vertical, or diagonal row wins the game. If all cells are filled without a winner, the game results in a draw.

## Features

- **Interactive Board**: A 3x3 grid where players can click to place their mark (X or O).
- **Two-player Mode**: The game alternates between player X (human) and player O (AI).
- **AI Opponent**: The AI opponent plays optimally using the Minimax algorithm.
- **Winner Detection**: The game checks for a winner after each move and declares if a player has won.
- **Draw Detection**: If all cells are filled and no one has won, the game declares a draw.
  
## Technologies Used

- **HTML**: Used to create the game structure, including the grid and buttons.
- **CSS**: Basic styling to arrange the grid and provide visual feedback.
- **JavaScript**: Implements the game logic, player turns, winner detection, and the AI algorithm.

## How It Works

### Game Board

The board consists of 9 cells, each represented by a `<div>` element. The cells are styled using CSS Grid for a 3x3 layout. Clicking on a cell triggers the game logic.

### Player Turns

- The player (X) starts first and clicks on any empty cell to place their mark.
- After each valid move, the AI (O) automatically takes its turn by calculating the best move using the Minimax algorithm.

### Winning and Drawing

- After each turn, the game checks for a winner by comparing the current board configuration to predefined winning combinations (rows, columns, and diagonals).
- If all cells are filled and no winner is found, the game declares a draw.

### AI Opponent (Minimax Algorithm)

The AI uses the Minimax algorithm to evaluate the best possible move:
- **Minimax** is a recursive algorithm used for decision-making and game theory.
- It simulates all possible moves and their outcomes, choosing the move that maximizes its chance of winning while minimizing the player's chance.
- The algorithm evaluates the game board based on winning or losing combinations and selects the optimal move for the AI.

## How to Use

1. **Open the HTML file** in a modern browser.
2. Player X starts by clicking on any empty cell.
3. The game alternates turns between Player X (human) and Player O (AI).
4. If Player X or O wins, an alert is shown declaring the winner.
5. If all cells are filled without a winner, an alert will indicate a draw.

## How the AI Works

- The AI evaluates each possible move using the Minimax algorithm.
- The algorithm simulates the game tree by alternating between maximizing (AI’s turn) and minimizing (player’s turn) moves.
- It assigns scores to each move (1 for a win, -1 for a loss, 0 for a draw) and picks the move with the highest score.
  
## Limitations

- The current implementation doesn't provide a reset button after the game ends. You need to refresh the page to start a new game.
- The game doesn't track player scores or provide advanced features like difficulty levels.

## Future Improvements

- **Reset Functionality**: Add a button to reset the board after a game ends.
- **Player Score Tracking**: Implement a score counter to keep track of wins, losses, and draws.
- **Difficulty Levels**: Add an option for the player to choose the difficulty level (easy, medium, hard) by adjusting the AI's behavior.
- **UI Enhancements**: Improve the visual design of the game to make it more engaging.

## License

This project is open-source and free to use or modify. Feel free to extend the functionality and improve the user experience.
