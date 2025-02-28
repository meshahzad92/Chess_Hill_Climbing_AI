# 🏰 N-Queens Problem Solver using Hill Climbing  

Solve the classic **N-Queens problem** using the **Hill Climbing algorithm**! This implementation efficiently finds a solution where no two queens threaten each other. 🎯♟️

---

## 📌 Problem Statement
The **N-Queens problem** requires placing **N queens** on an **N×N chessboard** so that **no two queens attack each other** (i.e., no two queens share the same row, column, or diagonal). 🏆

---

## 🚀 Approach
This solver utilizes the **Hill Climbing** algorithm to iteratively improve queen placements until a solution is found. 🏔️📈

### 🔹 Key Steps:
1. **Initialization:**
   - A **random initial state** is generated, where each column contains one queen at a random row.
   
2. **Objective Function:**
   - The **`calculateObjective`** function evaluates a board configuration by counting the number of **attacking queen pairs**.
   - The goal is to **minimize** this value to **zero**.
   
3. **Neighbor Generation:**
   - The **`getNeighbour`** function generates neighboring states by moving **one queen** in its column to another row.
   
4. **Hill Climbing Search:**
   - The **`hillClimbing`** function iteratively selects a **better neighboring state** (if available).
   - The process **stops at a local minimum**, where no better move exists.

---

## 📜 Code Structure

🔧 **Helper Functions:**
- **`configureRandomly`** → Initializes the board randomly.
- **`printBoard`** → Displays the current chessboard state.
- **`printState`** → Shows the queen positions.
- **`compareStates`** → Compares two states for equality.
- **`fill`** → Initializes the board with default values.
- **`calculateObjective`** → Computes attacking queen pairs.
- **`generateBoard`** → Converts state representation to board.
- **`copyState`** → Copies the state array.
- **`getNeighbour`** → Finds the best neighboring configuration.
- **`hillClimbing`** → Implements the Hill Climbing search.

---

## 🛠️ How to Use
This program is **self-contained** and can be executed directly. 🎯

1️⃣ **Run the script** 📜
2️⃣ The program **prints the final board** & **queen positions** 🏆
3️⃣ The number of attacking pairs is displayed (**ideally zero for a solution**) ✅

---

## ⚠️ Limitations & Challenges
❌ **Local Optima:** Hill Climbing can **get stuck** in a local minimum, failing to reach the global solution.  
❌ **No Backtracking:** Once at a local minimum, the algorithm **cannot recover** without modifications.  

🔹 **Possible Enhancements:**
✅ **Random Restarts** → Run the algorithm multiple times with different starting positions. 🔄  
✅ **Simulated Annealing** → Introduce randomness to escape local optima. 🔥  
✅ **Genetic Algorithms** → Evolve populations for a better solution. 🧬

---

## 📜 License
This project is released under the **MIT License**. Feel free to use, modify, and share it! 🚀  

