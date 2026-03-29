# 🎮 Tic Tac Toe - The Panda Edition

A clean, responsive, and interactive Tic Tac Toe game built with vanilla JavaScript, CSS Grid, and a touch of personality.


## 🌟 Features
* **Responsive Design:** Fully playable on desktops, tablets, and mobile devices thanks to CSS Media Queries.
* **Interactive UI:** Hover effects on the grid and smooth transitions for a modern feel.
* **Win Detection:** Real-time logic checks for winning combinations after every move.
* **Audio Feedback:** Catchy sound effects for each turn and game-over state.
* **Victory Celebration:** A hidden dancing panda appears once a player wins the match!
* **Reset Functionality:** Quickly clear the board and start a fresh game with a single click.

## 🛠️ Tech Stack
* **HTML5:** Semantic structure for the game layout.
* **CSS3:** Custom styling using **CSS Grid** for the board and **Flexbox** for alignment.
* **JavaScript (ES6):** Core game logic, including turn-tracking and DOM manipulation.

---

## 🧠 How It Works

### The Winning Logic
The game uses a pre-defined array of arrays representing the indices of the winning combinations on a 3x3 grid:

```javascript
const wins = [
    [0, 1, 2], [3, 4, 5], [6, 7, 8], // Rows
    [0, 3, 6], [1, 4, 7], [2, 5, 8], // Columns
    [0, 4, 8], [2, 4, 6]             // Diagonals
];
```

The `checkWin()` function iterates through these possibilities. If all three positions in a set contain the same character (and aren't empty), a winner is declared.

### Dynamic Styling
To keep the UI clean, the "Win Image" (the panda) is set to `0px` width by default. JavaScript dynamically updates the CSS width to `200px` only when the `isgameover` state becomes true.

---

## 🚀 How to Run Locally

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/TIC-TAC-TOE.git
    ```
2.  **Navigate to the folder:**
    ```bash
    cd TIC-TAC-TOE
    ```
3.  **Open the game:**
    Simply open `index.html` in your favorite web browser.

---

## 📈 Future Improvements
* [ ] Add a "Draw" detection logic for when the board is full.
* [ ] Implement an Unbeatable AI using the **Minimax Algorithm**.
* [ ] Add a score tracker to keep count of wins for Player X and Player 0.

---

