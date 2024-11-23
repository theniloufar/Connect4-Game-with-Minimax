# Connect4 Game with Minimax Algorithm

## Project Overview

This project implements a **Connect4** game featuring a human player versus a computer AI that uses the **Minimax Algorithm**. The AI player is designed with options for alpha-beta pruning and configurable search depth, allowing for performance tuning and comparison. The game also includes a graphical user interface (GUI) created with **Pygame** to visualize gameplay.

---

## Features

### 1. **Minimax Algorithm**
- The computer AI employs the Minimax algorithm to evaluate moves, aiming to maximize its chances of winning.
- Includes **Alpha-Beta Pruning** to reduce computational complexity, making the algorithm more efficient.

### 2. **Game Modes**
- **Human vs. CPU**: Human player competes against the AI.
- **Simulation Mode**: Run multiple games to test the performance of the algorithm.

### 3. **Performance Tuning**
- Adjustable **Minimax Depth** to balance between computational effort and gameplay quality.
- Toggle **Pruning** on or off to compare its impact on runtime and efficiency.

### 4. **Graphical User Interface**
- A GUI built with **Pygame** to provide a visual representation of the Connect4 board and game states.
- Highlights the winning player and displays results at the end of the game.

---

## Key Implementation Details

### Alpha-Beta Pruning
When enabled, the algorithm skips unnecessary branches during the Minimax tree evaluation, significantly reducing nodes visited:
- Example stats (depth 3):
  - **Pruning Enabled**: ~1346 nodes visited, runtime ~1.89 seconds.
  - **Pruning Disabled**: ~74200 nodes visited, runtime ~13.80 seconds.

### Simulation and Testing
The script includes a simulation mode for performance analysis. It can simulate hundreds of games at various depths, logging:
- Average runtime
- Nodes visited
- CPU and player winning probabilities

Run simulation:
```python
check_results()
```

---

## Insights from the Report

### Observations
1. **Pruning**:
   - Improves efficiency without sacrificing decision quality.
   - Reduces runtime and nodes visited exponentially.

2. **Depth vs Performance**:
   - Increasing depth enhances AI decision-making but at the cost of higher computation time.

3. **Alternative Algorithms**:
   - The current Minimax approach assumes an optimal opponent. For random opponents, **Monte Carlo Tree Search (MCTS)** is recommended.

---

Feel free to reach out for questions or suggestions! 🎮
