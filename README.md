# Hangman Game 

A console‑based Hangman game built in Python. This implementation lets a player guess a secret word one letter at a time. Wrong guesses are penalized more for vowels than for consonants, and the game calculates a final score.

---

## How the Game Works

1. A **secret word** (e.g. `"apple"`) is set in the code.  
2. The player starts with **6 guesses**.  
3. On each turn:  
   - The game shows how many guesses remain.  
   - It displays the letters that have not been guessed yet.  
   - It shows the current guessed word (with letters + `_` for missing ones).  
4. When the player guesses:  
   - If the letter was already guessed, nothing is deducted.  
   - If the guess is correct, the letter appears in the word.  
   - If the guess is wrong:  
     - **Vowels** (`a, e, i, o, u`) → **–2 guesses**  
     - **Consonants** → **–1 guess**  
5. The game ends when:  
   - The player guesses the entire word → they **win** and get a score.  
   - Or they run out of guesses → they **lose** and the secret word is revealed.  
6. **Score** = (remaining guesses) × (number of unique letters in the secret word)

---

## How to Run

- Open `HangMan_Game_ASSIGNMENT_NEW.ipynb` in Jupyter Notebook.  
- Run all the cells, then play when the `hangman('apple')` cell executes.  
- (If you convert to `.py`), run:  
  ```bash
  python hangman.py
