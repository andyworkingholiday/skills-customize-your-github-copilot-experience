# 📘 Assignment: Hangman Game

## 🎯 Objective

Build the classic word-guessing game using Python strings, loops, and user input. Create a Hangman game where players guess letters to reveal a hidden word before running out of attempts. You'll practice string manipulation, loops, conditionals, and random selection.

## 📝 Tasks

### 🛠️ Game Setup and Word Selection

#### Description
Initialize the game by randomly selecting a word from a predefined list and setting up the game state with remaining attempts.

#### Requirements
Completed program should:

- Maintain a predefined list of words to choose from
- Randomly select a word at the start of the game
- Initialize remaining attempts (e.g., 6 incorrect guesses allowed)
- Display the initial game state with blanks (e.g., `_ _ _ _ _` for a 5-letter word)

### 🛠️ Player Input and Validation

#### Description
Accept letter guesses from the player and validate that they are valid input.

#### Requirements
Completed program should:

- Prompt the player to enter a letter
- Validate that input is a single letter
- Handle duplicate guesses appropriately (either reject or track them)
- Continue prompting until a valid letter is provided

### 🛠️ Game Logic and Progress Display

#### Description
Process player guesses, update game progress, and display the current state of the word.

#### Requirements
Completed program should:

- Check if the guessed letter is in the word
- Update the display to show correctly guessed letters
- Keep track of incorrect guesses
- Decrement remaining attempts for incorrect guesses
- Display current progress, remaining attempts, and incorrect guesses after each turn

### 🛠️ Game Flow and Win/Lose Conditions

#### Description
Implement the overall game loop and determine when the game ends with a win or loss.

#### Requirements
Completed program should:

- Continue the game loop until the word is guessed or attempts run out
- Display a win message when the player guesses the complete word
- Display a lose message when attempts are exhausted and reveal the word
- Offer to play again after the game ends
- Example output:
  ```
  Congratulations! You guessed the word: PYTHON
  ```
  or
  ```
  Game Over! The word was: PYTHON
  ```
