# Maze Solving Program

![Maze Solving GIF](https://github.com/Nader-albaire/Maze-Solving-Program/blob/main/Picture_maze_solving.gif)

## Overview

This project is a maze-solving program implemented using Python and the Turtle graphics library. The program generates a maze, visualizes it, and solves it using the Breadth-First Search (BFS) algorithm. The maze-solving process is visually represented, showing the pathfinding progress and the final solution.

## Features

- **Maze Generation:** The program generates a maze from a predefined grid.
- **Maze Visualization:** The maze is visualized using Turtle graphics.
- **Breadth-First Search (BFS) Algorithm:** The program uses the BFS algorithm to find the shortest path from the start to the end of the maze.
- **Pathfinding Visualization:** The pathfinding process is visualized step-by-step.
- **Completion Indicator:** The program marks the start, end, and the path found.

## Program Description

### Classes

- **Maze:** Represents the maze structure. It uses a turtle to draw the maze on the screen.
- **Green:** Represents the finish line or the end point of the maze.
- **Blue:** Represents the pathfinding process (commented out in the final version but can be enabled for debugging).
- **Red:** Represents the starting point of the maze.
- **Yellow:** Represents the solution path from the start to the end of the maze.

### Grid

The maze is defined by a grid where:
- `+` represents walls.
- ` ` (space) represents paths.
- `s` represents the start point.
- `e` represents the end point.

### Main Functions

- **setup_maze(grid):** Sets up the maze by reading the grid and placing the walls, paths, start, and end points.
- **search(x, y):** Implements the BFS algorithm to find the shortest path from the start to the end.
- **backRoute(x, y):** Traces back the path from the end to the start and marks it.

### Execution Flow

1. The program initializes the screen and turtle objects.
2. It sets up the maze using the `setup_maze` function.
3. It starts the BFS search from the start point using the `search` function.
4. Once the end point is reached, it traces back the solution path using the `backRoute` function.
5. The program waits for the user to click on the screen to exit.

## Sample Mano Script and ASCII Codes

### Mano Script

```assembly
ORG 100
LOAD X
ADD Y
STORE Z
HALT
X, DEC 5
Y, DEC 10
Z, DEC 0
END
ASCII Codes
+ (Plus): ASCII Code 43
(Space): ASCII Code 32
s (Lowercase S): ASCII Code 115
e (Lowercase E): ASCII Code 101
Authors
Nader Albaire
Ishtiag Abbaker
How to Run
Make sure you have Python installed on your system.
Install the Turtle graphics library if it's not already installed.
Clone the repository from GitHub:
bash
Copy code
git clone https://github.com/Nader-albaire/Maze-Solving-Program.git
Navigate to the project directory:
bash
Copy code
cd Maze-Solving-Program
Run the program:
Copy code
python maze_solver.py
Enjoy solving the maze!
