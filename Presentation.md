# Flappy Bird Game in C++

## Description
This is a console-based implementation of the popular Flappy Bird game written in C++. The player controls a bird character made of ASCII characters and must navigate through pipe obstacles by timing jumps correctly. The game features classic Flappy Bird gameplay adapted for the Windows console environment with score tracking, random pipe generation, and collision detection.

## Features
- Console-based graphics with ASCII characters
- Menu system with game, instructions, and quit options
- Bird character that responds to gravity and jumps
- Randomly generated pipes with varying gap positions
- Score tracking as you successfully navigate through pipes
- Pause functionality during gameplay
- Game over screen with final score display

## Data Structure Analysis
This game utilizes several data structures for game logic:
- **Arrays (`pipePos[]`, `gapPos[]`, `pipeFlag[]`)**: Store the positions and states of the pipes and gaps
- **2D Character Array (`bird[][]`)**: Represents the ASCII art of the bird character
- **Integer Variables (`birdPos`, `score`)**: Track the bird's vertical position and player's score
- **Constants (`SCREEN_WIDTH`, `SCREEN_HEIGHT`, `WIN_WIDTH`, `GAP_SIZE`)**: Define the game boundaries and pipe characteristics
- **Windows API Structures (`COORD`, `CONSOLE_CURSOR_INFO`)**: Handle console cursor positioning and visibility

## Controls
```
Spacebar - Make the bird jump/flap
P - Pause/resume the game
ESC - Exit to main menu
```

## How to Run
1. Compile the code using a C++ compiler (such as g++ or Visual Studio)
2. Run the compiled executable in a Windows console window
3. Use the menu to start the game or view instructions

## Compilation Instructions
Using g++:
```sh
g++ flappy_bird.cpp -o flappy_bird.exe
```
Run the executable:
```sh
./flappy_bird.exe
```

## Game Logic
1. The game starts with a menu screen offering options to play, view instructions, or quit
2. The bird automatically falls due to simulated gravity
3. The player presses spacebar to make the bird jump upward
4. Pipes with random gap positions move from right to left across the screen
5. The player must navigate the bird through the gaps in the pipes
6. A point is earned each time the bird successfully passes through a pipe
7. The game ends if the bird collides with a pipe or the screen boundaries
8. The game over screen displays the final score

## Dependencies
- Windows Console (for `windows.h` functions)
- Standard C++ libraries (iostream, conio.h, stdlib.h, string.h, time.h)

## Known Issues
- The game is Windows-specific due to its use of Windows.h
- Screen flickering may occur due to console rendering limitations
- No persistent high score system

## Future Improvements
- Add color support for better visual experience
- Enhance pause functionality with a detailed pause menu
- Implement difficulty levels with adjustable pipe speed and gap size
- Add high score system with persistent storage
- Include sound effects for jumping, scoring, and game over
- Refactor code using object-oriented design principles
- Implement double buffering to reduce screen flickering
- Create cross-platform compatibility
- Add animated bird character with flapping wings

## Author
This code was sourced from a GitHub repository. This presentation was created as part of an analysis and documentation project.

## License
The original code is subject to the license terms specified by its original author on GitHub. This documentation is provided for educational and analytical purposes only.
