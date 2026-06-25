# 🟡 Pac-Man in Maze World

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python">
  <img src="https://img.shields.io/badge/Data%20Structures-Stack-success">
  <img src="https://img.shields.io/badge/Algorithm-DFS-orange">
  <img src="https://img.shields.io/badge/License-MIT-green">
</p>

A stack-based maze navigation system inspired by the classic **Pac-Man** game. The project finds a safe path for Pac-Man through a 2D maze while avoiding ghosts using **Depth First Search (DFS)** implemented with a **custom Stack**.

---

## 📖 Overview

In this project, Pac-Man must travel from a starting position to a destination while avoiding cells occupied by ghosts.

The maze is represented as a **2D grid**, where:

- `0` → Empty cell
- `1` → Ghost (blocked cell)

The navigator searches for a valid path without revisiting any cell.

If no path exists, the program throws a `PathNotFoundException`.

---

## ✨ Features

- 🟨 Custom Maze implementation
- 👻 Add and remove ghosts dynamically
- 🧭 Stack-based DFS pathfinding
- 🚫 Prevent revisiting cells
- ⚠️ Exception handling when no path exists
- 📊 Efficient traversal with linear time complexity
- 🧱 Object-Oriented Design

---

## 🖼️ Project Demo

<p align="center">
  <img src="https://github.com/user-attachments/assets/9b287dcc-54a0-4758-8bc0-667b36eb884e" width="420">
  <img src="https://github.com/user-attachments/assets/c332495e-b0b9-4d34-96d2-a993690e244f" width="420">
</p>

---

# 🧠 Algorithm

The navigator performs **Depth First Search (DFS)** using a custom Stack.

### Steps

1. Push the starting cell onto the stack.
2. Mark it as visited.
3. Repeatedly:
   - Pop the top cell.
   - Check whether it is the destination.
   - Push all valid neighbouring cells.
4. Continue until:
   - Destination is found.
   - Stack becomes empty.

If the stack becomes empty before reaching the destination, a `PathNotFoundException` is raised.

---

# 📊 Time Complexity

| Operation | Complexity |
|-----------|------------|
| DFS Traversal | **O(N × M)** |
| Space Complexity | **O(N × M)** |

where **N × M** is the maze size.

---

# 🏗️ Project Structure

```
Pac-Man-in-Maze-World/
│
├── maze.py
├── navigator.py
├── stack.py
├── exception.py
├── main.py
└── README.md
```

---

# 📂 File Description

### maze.py

Implements the Maze class.

Functions include:

- Add ghosts
- Remove ghosts
- Check blocked cells
- Print maze

---

### navigator.py

Contains the DFS navigation algorithm.

Responsible for:

- Path searching
- Maintaining visited cells
- Returning the final path
- Throwing exceptions

---

### stack.py

Custom implementation of Stack.

Supports:

- Push
- Pop
- Peek
- isEmpty

---

### exception.py

Contains:

```
PathNotFoundException
```

Raised whenever a valid path cannot be found.

---

### main.py

Entry point for running and testing the project.

---

# 🎮 Sample Input

Maze

```
0 1 0 0
0 0 0 0
0 0 1 0
0 1 0 0
```

Start

```
(2,0)
```

Destination

```
(2,3)
```

---

# ✅ Output

```
[(2,0),
 (2,1),
 (1,1),
 (1,2),
 (1,3),
 (2,3)]
```

---

# 🛠️ Tech Stack

- Python
- Object-Oriented Programming
- Stack Data Structure
- Depth First Search (DFS)

---

# 🚀 Getting Started

Clone the repository

```bash
git clone https://github.com/dhanoliya-ji/Pac-Man-in-Maze-World.git
```

Go to the project

```bash
cd Pac-Man-in-Maze-World
```

Run

```bash
python main.py
```

---

# 💡 Future Improvements

- 🎮 Interactive GUI using Pygame
- 🤖 Multiple ghost movement
- ⚡ BFS shortest-path mode
- 🌟 A* Search implementation
- 🎵 Sound effects and animations

---

# 📚 Concepts Covered

- Depth First Search
- Stack
- Graph Traversal
- Backtracking
- Object-Oriented Programming
- Exception Handling

---

# 👨‍💻 Author

**Gajendra Dhanoliya**

B.Tech, IIT Delhi

If you found this project helpful, consider giving it a ⭐ on GitHub.
