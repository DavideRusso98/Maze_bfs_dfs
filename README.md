# Maze BFS & DFS 🧩🔍

This project focuses on solving randomly generated **mazes** using two fundamental search algorithms: **Breadth-First Search (BFS)** and **Depth-First Search (DFS).**

![Screenshot 2025-06-05 alle 13 15 10](https://github.com/user-attachments/assets/83a27d8d-cc9c-4611-bb24-b584b8cba840)

## 🔍 Breadth-First Search (BFS)

**BFS** is a graph traversal algorithm that explores vertices in the order of their distance from the starting point, ensuring that all nodes at the current depth level are visited before moving to the next level.

-   **Data Structure Used:** Queue (FIFO - First In, First Out).
    
-   **Traversal Strategy:** Starting from the **root** node, BFS visits all neighboring nodes. Then, for each of those nearest nodes, it explores their unexplored neighbors, and so on. This process continues until all nodes have been visited.
    
-   **Shortest Path:** In unweighted graphs, BFS guarantees the **shortest path** from the starting node to all other nodes.
    
**Time and Space Complexity:**

-   **Time Complexity:** O (V + E), where V is the number of vertices and E is the number of edges.
    
-   **Space Complexity:** O (V), due to the storage of vertices in the queue.

## 🔍 Depth-First Search (DFS)

**DFS** is a graph traversal algorithm that explores as far as possible along each branch before backtracking, diving deep into the graph's branches.

-   **Data Structure Used:** Stack (LIFO - Last In, First Out), which can be implemented using recursion.
    
-   **Traversal Strategy:** Starting from the **root** node, DFS explores as far as possible along each branch before backtracking. This means it goes **deep** into the graph and backtracks when it hits a node with no unvisited neighbors.
    
-   **Path Finding:** DFS does **not** guarantee the shortest path in graphs.
    
**Time and Space Complexity:**

-   **Time Complexity:** O (V + E), similar to BFS.
    
-   **Space Complexity:** O (V) in the worst case, due to the storage of vertices in the stack or recursion call stack.

## 📊 Comparative Analysis: 

| Feature              | BFS                                                      | DFS                                                      |
|----------------------|-----------------------------------------------------------|-----------------------------------------------------------|
| **Data Structure**   | Queue                                                     | Stack (or recursion)                                      |
| **Traversal Strategy**| Level by level                                            | Depth-wise (deep into branches)                           |
| **Shortest Path**    | Yes (in unweighted graphs)                                | No                                                        |
| **Memory Usage**     | Can be high (stores all nodes at current level)           | Generally lower (stores nodes along current path)         |
| **Completeness**     | Complete (will find a solution if one exists)             | Not complete in infinite graphs                           |
| **Optimality**       | Optimal for unweighted graphs                             | Not guaranteed to be optimal                              |
| **Use Cases**        | Shortest path, broadcasting, web crawling                 | Topological sort, cycle detection, puzzles                |

## 📁 Project Structure

The project is organized as follows:

### 🧩 `src/maze/`
Contains classes related to the maze's structure and generation:

- `Maze.java`: Represents the maze grid and its properties.
- `Cell.java`: Defines individual cells within the maze.
- `MazeGenerator.java`: Handles the procedural generation of the maze.

### 🔍 `src/algorithms/`
Implements the search algorithms used to solve the maze:

- `BFS.java`: Implements the Breadth-First Search algorithm.
- `DFS.java`: Implements the Depth-First Search algorithm.

### 🖥️ `src/gui/`
Manages the graphical user interface components:

- `MazePanel.java`: Responsible for rendering the maze and the solution paths.
- `MainFrame.java`: Sets up the main application window and integrates all components.

## 🖥️ Graphical User Interface

![Screenshot 2025-06-05 alle 13 15 10](https://github.com/user-attachments/assets/83a27d8d-cc9c-4611-bb24-b584b8cba840)


