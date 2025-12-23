# Rock Paper Scissors Game 🎮

A classic Rock-Paper-Scissors console game written in C++ where you can compete against the computer in multiple rounds!

## Description

This is a console-based implementation of the traditional Rock-Paper-Scissors game. Challenge the computer to a best-of match with up to 10 rounds. The game features colorful console output and detailed statistics tracking to make your gaming experience more engaging.

## Features

- **Multiple Rounds**: Play 1-10 rounds per game
- **Interactive Gameplay**: Choose your move each round (Stone, Paper, or Scissors)
- **Smart Computer Opponent**: Computer makes random choices each round
- **Visual Feedback**: Console colors change based on round results
  - 🟢 Green: Player wins
  - 🔴 Red: Computer wins  
  - 🟡 Yellow: Draw
- **Detailed Statistics**: Track wins, losses, and draws
- **Play Again Option**: Continue playing without restarting the program
- **Sound Alert**: Audio notification when computer wins

## Game Rules

- **Stone** beats **Scissors**
- **Paper** beats **Stone**
- **Scissors** beats **Paper**
- Same choices result in a **Draw**

## Requirements

- **Compiler**: C++11 or later
- **IDE**: Visual Studio 2022 (recommended) or any C++ compiler
- **OS**: Windows (uses `system("color")` and `system("cls")` commands)

## How to Build and Run

### Using Visual Studio 2022

1. Open Visual Studio 2022
2. Go to `File` → `Open` → `Project/Solution`
3. Select the `.sln` file
4. Press `F5` or click `Debug` → `Start Debugging`

### Using Command Line (g++)

```bash
g++ -std=c++11 rock_paper_scissors.cpp -o RockPaperScissors
./RockPaperScissors
```

### Using Command Line (MSVC)

```cmd
cl /EHsc rock_paper_scissors.cpp
RockPaperScissors.exe
```

## How to Play

1. Run the program
2. Enter the number of rounds you want to play (1-10)
3. For each round, choose your move:
   - Press `1` for Stone
   - Press `2` for Paper
   - Press `3` for Scissors
4. View the round results and current score
5. After all rounds, see the final game statistics
6. Choose whether to play again (Y/N)

## Sample Gameplay

```
How Many Rounds 1 To 10 ?
5

Round [1] Begins:

Your Choice: [1]:Stone, [2]:Paper, [3]:Scissors ? 1

_________________Round [1] _________________

Player Choice   : Stone
Computer Choice : Scissors
Round Winner    : [Player1]
__________________________________
```

## Project Structure

```
rock-paper-scissors/
│
├── rock_paper_scissors.cpp    # Main source code
├── README.md                   # This file
├── .gitignore                  # Git ignore file
└── *.sln                       # Visual Studio solution file
```

## Technical Details

### Data Structures

- **Enumerations**: 
  - `enGameChoice`: Represents player choices (Stone, Paper, Scissors)
  - `enWinner`: Represents round/game winners
  
- **Structures**:
  - `stRoundInfo`: Stores information about each round
  - `stGameResults`: Stores overall game statistics

### Key Functions

- `PlayGame()`: Main game loop
- `WhoWonTheRound()`: Determines round winner based on choices
- `WhoWonTheGame()`: Determines overall game winner
- `SetWinnerScreenColor()`: Changes console color based on results

## Contributing

Contributions are welcome! Here are some ideas for improvements:

- Add difficulty levels (Easy, Medium, Hard)
- Implement a streak counter
- Add lizard and Spock for Rock-Paper-Scissors-Lizard-Spock variant
- Save game history to a file
- Create a GUI version
- Add multiplayer mode

## License

This project is open source and available for educational purposes.
⭐ If you enjoyed this project, please give it a star on GitHub!



