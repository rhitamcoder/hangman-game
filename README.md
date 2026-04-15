# 🪓 Hangman CLI Game
A classic, lightweight word-guessing game built in Python. Designed for the terminal, this version of Hangman focuses on clean logic, interactive gameplay, and that nostalgic "low-fi" terminal aesthetic.

## 🌟 Features
### ASCII Visuals:
Dynamic drawing of the hangman as you progress through incorrect guesses.

### No-Install Design:
Runs directly via Python using standard libraries - no 'pip install' required.

### Minimalist Workflow:
Fast, keyboard-driven interface optimized for terminal enthusiasts.

### Modular Design:
Code is organized into three distinct files (Logic, Art and Words) for better readability.

### Extensive Word Bank:
Includes a dedicated word list file, making it easy to add or customize categories.

## 🚀 Installation & Setup
### 1. Download the Tool
Open your terminal and clone this repository:
```
git clone https://github.com/rhitamcoder/hangman-game.git
```
```
cd hangman-game
```
*(Alternatively, click the green **Code** button on Github and select **Download ZIP**.)*

### 2. Create a Global Command
If you want to play the game by simply typing 'hangman' from any folder in your terminal, follow these steps into a new terminal window:

#### 1. Hide the folder:
```
mv hangman-game .hangman-game
```

#### 2. Create a launcher script:
```
sudo nano /usr/local/bin/hangman
```

#### 3. Paste the following logic (Replace /path/to/ with the actual path where you cloned the folder):
```
#!/bin/bash
cd /path/to/.hangman-game/ && python3 hangman.py
```

#### 4. Save and Exit:
Press 'Ctrl+O', 'Enter', then 'Ctrl+X'.

#### 5. Make it executable:
```
sudo chmod +x /usr/local/bin/hangman
```

## 🎮 How to Use
Simple open your terminal and type: 
```
hangman
```

### Manual Run
If you did not set up the global command, simply navigate to the folder and run:
```
python3 hangman.py
```

### The Logic
**1. The Objective:** Guess the hidden word one letter at a time before the hangman is fully drawn.
**2. Input:** Type a single letter and press 'Enter'.
**3. Feedback:** The game will show you your correctly guessed letters and a list of missed attempts.
**4. Win/Loss:** If you complete the word, you win! If the hangman is finished (after 6 wrong guesses), the game is over.

## 🛠️ Requirements
**Python 3.x:** Works perfectly on any system with Python installed.
**Linux/Unix Optimized:** Tested on Arch, Ubuntu, Fedora, Mint, (Any Ubuntu-based distros) & MacOS.

## 🧠 Why I Built This
This project was a deep dive into Python logic loops and string manipulation. It's a tribute to the classic "pen & paper" games, reimagined for the command line to prove that you don't need a heavy GUI to have a fun, polished experience.

## 📈 Key Learnings
By building this CLI game, I focused on:
**1. Input Handling:** Managing user errors and ensuring the game doesn't crash on weird inputs.
**2. Game State Management:** Keeping track of lives, guessed letters, and the hidden word simultaneously.
**3. Terminal UI:** Using ASCII arts to provide visual feedback within a text-only environment.

### Contributing:
Feel free to Fork this repo to add your own word lists or custom ASCII art designs!
