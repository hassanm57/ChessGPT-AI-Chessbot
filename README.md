# ChessGPT: AI-Powered Chessbot

**Team Members:**
- **Hassan Mansoor** - CMS: 403544
- **Taha Ahmed Rasheed** - CMS: 412452
- **Ahsan Mohsin** - CMS: 409639

**Class:** BSCS12A

---

## 🔍 Introduction

ChessGPT is a project aimed at integrating artificial intelligence techniques into the classic game of chess. The objective was to create a chess engine capable of playing competitively against humans while offering features that make it accessible to players of varying skill levels. The project involves implementing traditional AI algorithms, such as the MinMax algorithm variant, NegaMax with Alpha-Beta pruning, and Position Evaluation Using Heuristics, to make strategic decisions.

![ChessGPT in action](![image](https://github.com/user-attachments/assets/d5657c65-5271-4724-8ea5-72ede940090e)
)
)

---

## 🛠️ Method

The development of ChessGPT focused on combining AI techniques with an intuitive user interface. The methodology is detailed below:

### 🔢 Algorithms Implemented

- **Negamax Algorithm:**  
  A variation of the MinMax algorithm optimized for two-player zero-sum games was used to evaluate possible moves. The algorithm alternates between maximizing the player’s advantage and minimizing the opponent’s advantage.

- **Alpha-Beta Pruning:**  
  This reduces the number of nodes evaluated by the Negamax algorithm, allowing deeper analysis within the same computational budget.

- **Evaluation Heuristic Functions:**  
  The AI evaluates board positions based on static heuristics, such as material value (piece strength), board control, and positional advantages like centrality and king safety.

- **Depth-Limited Search:**  
  Limits the recursive search to a predefined depth, allowing for a balance between strategy and computational complexity.

- **Randomized Move Selection:**  
  Includes a fallback mechanism to select a random valid move when a strategic decision cannot be made.

- **Recursive Backtracking:**  
  Uses recursion to explore all possible moves to a given depth, simulating “what-if” scenarios for both players.

- **Game State Evaluation:**  
  Explicit handling of checkmate and stalemate conditions to assign extreme scores (+1000 for checkmate and 0 for stalemate).

### 💻 Software Tools

- **Python:**  
  Chosen for its simplicity and availability of libraries for game development and numerical computation.

- **pygame:**  
  Used for building the graphical user interface to render the chessboard, pieces, and interactive gameplay.

- **NumPy:**  
  Employed to handle matrix operations and efficient data manipulation for the AI logic.

### 🎮 Game Features

ChessGPT includes several features:
- Adjustable difficulty levels, where the depth of the AI’s search can be configured.
- Undo and reset functionality, allowing users to explore different strategies.
- An interactive GUI for smooth gameplay and visual feedback.
- A log displayed alongside for move history.
- Piece possible moves highlighted on the board when clicked.
- Ability to choose to play as White or Black, with board flip functionality as well.
- Ability to drag/drop pieces to move as well as clicking.
- Functionality for Player vs. Player, AI vs. AI, or Player vs. AI.
- Various sound effects for piece moves, captures, checks, wins/losses.
- Pawn promotion and en passant move functionality.
- Functionality to check for pins, castling rights, and stalemates.

---

## 🏆 Discussion

### 🎯 Achievements

We achieved the primary objective of creating a functional AI chess engine. The Negamax algorithm with Alpha-Beta pruning, coupled with evaluating piece score heuristics, enabled efficient move exploration, providing competitive gameplay at various difficulty levels. The GUI was well received for its simplicity and responsiveness.

### ⚠️ Challenges and Enhancements

- **Performance Bottlenecks:**  
  Higher difficulty levels with deeper search depths occasionally caused delays, impacting the gameplay experience.

- **Static Evaluation Limitations:**  
  The evaluation function relies on predefined heuristics, which can limit the AI’s ability to understand complex positional dynamics.

- **Improvements To Add:**  
  We can integrate machine learning-based evaluation functions, using neural networks and dynamic difficulty to improve the performance of the chessbot.

## 🚀 Getting Started

Follow these steps to set up ChessGPT on your local machine:

### 1️⃣ Clone the Repository
First, clone the ChessGPT repository to your local machine:
```bash
git clone https://github.com/hassanm57/ChessGPT-AI-Chessbot
cd ChessGPT
```
# Install dependencies
```bash
pip install -r requirements.txt
```
# Run the game
```bash
python chess_ui.py


