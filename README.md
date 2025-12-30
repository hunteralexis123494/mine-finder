# mine_finder

C program simulating Minesweeper, allowing users to read board data from a file, generate a random board, or play interactively.

---

## Features

- Load board from a file
- Generate a random board
- Play interactively in basic mode
- Automatic calculation of neighboring mines
- Prints board with mines and numbers

---

## Project Structure
```
mine-finder/
│
├── main.c # Entry point for the game
├── functions.c # Implementation of game functions
├── functions.h # Function prototypes and constants
├── sample_board.txt # Sample board for demonstration
└── README.md
```
---

## Sample Data

`in1.txt` contains a 10x10 grid of zeros and ones (`1` indicates a mine) for testing the file input feature:

10 10
0 0 0 0 0 0 0 0 1 0
0 1 0 0 0 0 0 0 1 0
0 0 0 0 0 0 0 0 0 0
0 0 0 0 1 1 0 0 0 0
0 0 0 0 0 1 0 0 0 0
0 1 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 1 0 0
0 0 0 0 0 0 0 1 0 0
0 0 0 1 0 0 0 0 0 0

This allows testing the file-reading feature and demonstrating program functionality without generating a random board.

---

## Technologies Used

- C (C99 standard)
- Standard Library
- Terminal/CLI-based interaction

---

## How to Run

1. Clone the repository:
git clone https://github.com/hunteralexis123494/mine-finder.git

2. Navigate to the project directory:
cd mine-finder

3. Compile the program:
gcc main.c functions.c -o mine_finder

4. Run the program (example using sample board):
./mine_finder in1.txt output.txt

---

## Design Decisions

- Modularized functions for board generation, neighbor checking, and gameplay
- Input validation for user-entered board dimensions
- Separate file reading and random board generation for flexibility
- Interactive board display using characters to indicate mines and numbers

---

## Future Improvements

- Add advanced graphics interface or GUI
- Allow custom board sizes and mine counts
- Save/load game states
- Add difficulty settings and scoring system

---

## Author

Alexis Hunter
