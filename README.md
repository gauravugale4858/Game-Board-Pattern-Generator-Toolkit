# Tic-Tac-Toe with NumPy & Matplotlib

A two-player Tic-Tac-Toe game for Python. The board is stored as a NumPy array and drawn with Matplotlib. The script also includes a few small NumPy board demos (chessboard and diagonal patterns) that were written while building the game.

## Features

- 3x3 board represented as a NumPy array (`0` = empty, `1` = X, `2` = O)
- Matplotlib-rendered board that updates after every move
- Winner detection for rows, columns and both diagonals
- Draw detection when the board is full
- Input validation (out-of-range numbers, occupied cells, non-integer input)
- Extra NumPy demos: 8x8 chessboard, diagonal and anti-diagonal patterns

## Requirements

- Python 3.8+
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)

Install the dependencies:

```bash
pip install numpy matplotlib
```

## Usage

Clone the repository and run the script:

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
python game_board.py
```

> **Note:** The script first runs the NumPy demos, which open Matplotlib windows (chessboard, diagonal patterns, a sample board). Close each window to continue. The playable game starts at the end.

## How to Play

1. Player **X** goes first, then players alternate.
2. When prompted, enter a **row** (0-2) and a **column** (0-2).
3. The first player to get three in a row (horizontally, vertically or diagonally) wins.
4. If all nine cells are filled with no winner, the game is a draw.

Positions are zero-indexed:

```
(0,0) (0,1) (0,2)
(1,0) (1,1) (1,2)
(2,0) (2,1) (2,2)
```

## Code Overview

| Function | Description |
|---|---|
| `check_winner(board)` | Returns `1` if X wins, `2` if O wins, `0` if no winner yet |
| `display_board(board)` | Draws the board with Matplotlib |
| `play_game()` | Main game loop: input, validation, win/draw checks |

## Project Structure

```
.
├── game_board.py   # Game code and NumPy demos
└── README.md
```

## Possible Improvements

- Add an AI opponent (e.g. minimax)
- Click-to-play with Matplotlib mouse events instead of typing coordinates
- Move the demo code into a separate file
- Add a "play again" option

## License

This project is open source. Add a license of your choice (e.g. MIT) before publishing.
