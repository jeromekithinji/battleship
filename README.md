# Battleship Game

Welcome to the **Battleship Game**! This project is an implementation of a simplified version of the classic Battleship game, developed as part of an assignment for COMP6481 (Winter 2024). The program allows a human player to compete against a computer opponent in a turn-based grid battle.

---

## About the Game

The game is played on an 8x8 grid, where each player (human and computer):
- Places **6 ships** and **4 grenades** on the grid.
- The positions of the ships and grenades are hidden from the opponent.
- Takes turns "firing rockets" at positions on the grid, attempting to sink the opponent's ships.

### Game Rules
1. **Rocket Hits**:
   - If a rocket hits an opponent's ship, the ship is sunk.
   - If it hits a grenade, the player loses their next turn.
   - If it hits an empty position, nothing happens.
2. **Position Validity**:
   - Ships and grenades cannot overlap, and positions must fall within the 8x8 grid.
3. **Endgame**:
   - The game ends when one player's ships are all sunk. The remaining player is declared the winner.

---

## How It Works

1. **Setup**:
   - The human player places their ships and grenades on the grid by entering coordinates (e.g., `A1`, `C4`).
   - The computer randomly places its own ships and grenades, ensuring no overlaps.

2. **Gameplay**:
   - Players take turns firing rockets by entering coordinates.
   - The grid updates after each move, showing:
     - `S`: A computer ship hit.
     - `s`: A player ship hit.
     - `G`: A computer grenade hit.
     - `g`: A player grenade hit.
     - `*`: A position called but empty.

3. **Winning**:
   - The first player to sink all opponent ships wins.

4. **Final Display**:
   - After the game, the full grid (with all ships and grenades revealed) is shown for review.

---

## Learning Objectives

This project helps develop skills in:
- **Java Programming Basics**: Practice with loops, arrays, and classes.
- **Object-Oriented Design**:
  - Encapsulation, abstraction, and proper method decomposition.
  - Using enumerated types for clarity.
  - Managing a 2D array as a grid of objects.
- **Error Handling**: Ensuring valid inputs for grid positions and handling edge cases.
- **Game Design**: Creating an interactive and logical game flow.
- **Testing and Debugging**: Ensuring accuracy in gameplay mechanics.
- **JavaDoc Documentation**: Writing professional and clear documentation for the code.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository_url>

2. Compile the Java files:
    ```bash
    javac BattleshipGame.java

3. Run the program:
   ```bash
    java BattleshipGame
