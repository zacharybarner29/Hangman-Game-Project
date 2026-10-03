# Hangman Game
This game chooses a word from multiple languages and difficulty levels, and the user can win by getting a hint, guessing letters, or guessing the word. 
## Features
1. English, French, and Spanish words
2. Easy or hard difficulty levels
3. A scoring system (percentage)
## How It Works
1. The user enters the language and difficulty level
2. The game picks a random word from a list depending on the user's input
3. The user gets 6 guesses to find the correct word
   - Guess a letter
        - The game checks each index of the correct word to see if the letter guessed is in the correct word
    - Guess the whole word
        - If the user is wrong, they lose the game
    - Receive a hint (costs 3 guesses)
        - The game uses list slicing to only show the first two letters of the correct word
4. If the user guesses the word, they receive a message saying they won, and the points they received
5. If the user runs out of guesses or guesses the whole word wrong, they receive a message saying they lost and what the correct word was
## Challenges I Ran Into
- I kept running into a bug where the game would crash after the user's first guess. Eventually, I realized that my function was returning the user's correct guesses as a string, but when the function looped, it took the variable as a list. I fixed this by returning a list rather than a string. 
## What I'd Improve With More Time
- I would have incorporated more error handling and made my variable more efficient and easier to visually understand.
  
Made by Zachary Barner — https://github.com/zacharybarner29

