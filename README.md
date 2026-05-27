# 🔍 Search Algorithms in AI

Practical implementation of classic search algorithms in Python, using Jupyter Notebooks.

---

## 📁 Structure

```
search-algorithms/
├── task1_word_search.ipynb     # Word Search Puzzle Solver
├── task2_pathfinding_bfs.ipynb # Pathfinding with BFS
├── task3_maze_dfs.ipynb        # Maze Solving with DFS
└── README.md
```

---

## 📌 Tasks

### Task 1 — Word Search Puzzle Solver
> Find words in a 2D grid of letters (horizontal, vertical, diagonal, forward & reverse)

- `search_word(grid, word)` → searches one word in all 8 directions
- `find_words(grid, words)` → returns all found words from a list

### Task 2 — Pathfinding Basics (BFS)
> Find the shortest path from `S` to `E` on a grid with blocked cells `X`

- `is_valid(cell, grid)` → checks if a cell can be traversed
- `get_neighbors(cell, grid)` → returns valid adjacent cells
- `find_shortest_path(grid, start, target)` → BFS shortest path

### Task 3 — Maze Solving (DFS)
> Navigate a maze from `S` to `E` using recursive depth-first search

- `dfs(maze, row, col, visited, solution_path)` → recursive DFS
- `solve_maze(maze)` → returns solution path or empty list

---

## ⚙️ Setup

```bash
pip install git+https://github.com/mehalyna/cooltest.git
```

---

## 🗺️ Grid legend

| Symbol | Meaning      |
|--------|--------------|
| `S`    | Start point  |
| `E`    | End / Exit   |
| `X`    | Blocked cell |
| ` `    | Open path    |

---

## 🧠 Algorithm Comparison

| Algorithm | Task | Shortest Path | Strategy        |
|-----------|------|:-------------:|-----------------|
| BFS       | 2    | ✅ Yes        | Level by level  |
| DFS       | 3    | ❌ No         | Depth first     |

---

## 🧪 Testing

Each notebook includes an **interactive input cell** to test with custom words, coordinates, or mazes directly in Jupyter.

Tests run automatically via `@test_*` decorators from `cooltest`.