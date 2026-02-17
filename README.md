# AI Pathfinder – Blind Search Visualizer

A Python-based interactive visualizer for **uninformed / blind search algorithms** on a grid.
Explore and compare how different algorithms explore nodes and find paths in a grid with static obstacles.

---

## **Features**

* Visualizes step-by-step execution of:

  * Breadth-First Search (BFS)
  * Depth-First Search (DFS)
  * Uniform Cost Search (UCS)
  * Depth-Limited Search (DLS)
  * Iterative Deepening DFS (IDDFS)
  * Bidirectional Search
* Displays:

  * Explored nodes
  * Frontier nodes
  * Final path (if found)
  * Step statistics
* Customizable grid, start and goal positions, and static walls.
* Clockwise neighbor traversal including diagonals.

---

## **Requirements**

* Python **3.x** (tested on Python 3.14)
* Python packages:

  * `matplotlib`

> ⚠ **Note:** This code does **not require Pygame**, only Matplotlib for visualization.

---

## **Installation**

1. **Check Python installation**

```bash
python --version
```

2. **Install Matplotlib**

```bash
pip install matplotlib
```

> If `pip` is not recognized, follow the steps to [install pip](https://pip.pypa.io/en/stable/installation/).

---

## **Running the Visualizer**

1. Open a terminal / command prompt in the project directory.
2. Run the main script:

```bash
python pathfinder.py
```

3. Follow the on-screen menu to choose an algorithm (1-6) or quit (`q`).
4. The visualizer will animate the search process and display statistics.
5. After completion, you can run another algorithm by entering `y` or exit with `n`.

---

## **Controls / UI**

* The legend shows symbols for:

  * `S` – Start node
  * `T` – Goal node
  * `■` – Static wall
  * `F` – Frontier nodes
  * `·` – Explored nodes
  * `★` – Final path
* The stats panel displays:

  * Algorithm name
  * Current step
  * Nodes explored
  * Frontier size
  * Path found status
  * Path length (if found)
* Move order in traversal:
  **↑  →  ↓  ↘  ←  ↖** (strict clockwise order including diagonals)

---

## **Grid Configuration**

* Default grid: 10x10
* Start: `(1,1)`
* Goal: `(8,8)`
* Static walls:

```
(2, 3), (3, 3), (4, 3), (4, 4), (4, 5),
(6, 5), (6, 6), (6, 7), (5, 7), (3, 7)
```

* Directions:

```
1. Up      (-1, 0)
2. Right   (0, 1)
3. Down    (1, 0)
4. Diagonal Down-Right (1,1)
5. Left    (0, -1)
6. Diagonal Up-Left (-1,-1)
```

---

## **License**

This project is free to use and modify for educational purposes.

---
