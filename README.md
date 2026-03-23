# Kalaha Terminal Game

## Course Submission Overview

This project is a terminal-based implementation of the board game **Kalaha** ,a variant of Mancala. The program allows a human player to compete against a computer-controlled opponent. The AI opponent uses the **Minimax algorithm with alpha-beta pruning** to select its moves.

This submission is written in **Python 3** and therefore does **not require compilation** in the traditional sense. The program only needs to be executed from a terminal.



## Requirements

To run the game, the following is required:

- **Python 3** installed on the system
- A terminal or command prompt
- No external libraries or additional packages are required



## How to Run the Program
Clone the project

```bash
  git clone https://link-to-project
```

1. Open the folder contaiining the project.
2. Open a terminal or command prompt in that folder.
3. Run the following command:

```bash
python main.py
```

If the system uses `python3` instead of `python`, run:

```bash
python3 main.py
```

Once started, the game will display the board in the terminal and prompt the human player for input.



## How to Play

- The human player is **Player 1**.
- The computer opponent is **Player 2**.
- On each turn, the human player must enter a number from **1 to 6** corresponding to one of their pits.
- The AI automatically chooses a move on its turn.
- The game ends when one player's six pits are empty.
- Any remaining stones on the opposite side are moved to that player's store.
- The winner is the player with the higher number of stones in their store at the end of the game.

If an invalid input is entered, the program will request a new input.



## Board Representation

The board is displayed in the terminal using two rows:

- The **top row** represents the pits belonging to **Player 2 (AI)**
- The **bottom row** represents the pits belonging to **Player 1 (human)**
- `[P2:x]` represents Player 2's store
- `[P1:x]` represents Player 1's store

The pit numbering shown to the human player is **1 to 6** from left to right on the player's own side.



## Submitted Files

The project consists of the following files:

- `main.py` — entry point of the program; handles game flow and terminal interaction
- `board.py` — implementation of the Kalah board and core game rules
- `ai.py` — implementation of the AI opponent using Minimax with alpha-beta pruning
- `ai_test.py` — duplicate copy of the AI implementation used for testing purposes

