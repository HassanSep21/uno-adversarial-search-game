# GAME AI - UNO using Adversarial Search

A simplified UNO game simulation built in Python, featuring AI agents powered by Minimax and Expectimax algorithms. This project demonstrates adversarial search techniques through varying player strategies.

## Game Setup & Agents

The game consists of three players, each with distinct logic and play styles:

* **Player 1 (Defensive AI):** Uses the **Minimax** algorithm (Depth 3). Focuses on minimizing opponents' scores, managing 'Skip' cards, and keeping opponents' card counts high.
* **Player 2 (Offensive AI):** Uses the **Expectimax** algorithm (Depth 3). Focuses on aggressive card shedding. Treats drawing a card as a chance node, calculating expected values based on remaining deck probabilities.
* **Player 3 (Simulation):** Acts as an observer mode using the Minimax algorithm to simulate a full AI vs. AI vs. AI game environment.

## Rules Implemented
* **Standard Matching:** Play a card of the same color or value.
* **Drawing:** If no valid card exists, the player must draw one card.
* **Skip Card:** Skips the next player's turn.
* **Winning Condition:** The first player to reach 0 cards wins. 

## How to Run

The game requires no external dependencies. It uses Python's standard libraries (`random`, `copy`, `collections`).

1. Clone the repository.
2. Run the main Python script:
   ```bash
   python uno_ai.py
3. The terminal will output the step-by-step game simulation, including tree depth evaluations, expected scores, and AI decisions.