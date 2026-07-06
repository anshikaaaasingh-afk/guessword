# Word Guess 🔤

A simple terminal-based word guessing game (Hangman-style) built in Python.
Guess the hidden word one letter at a time before you run out of tries!

## How It Works

- The game picks a random word from a built-in word list.
- The word is displayed as underscores (`_ _ _ _ _`), one per letter.
- You guess one letter at a time.
- Correct guesses reveal the letter in the word.
- Wrong guesses cost you one of your 6 tries.
- Win by revealing the whole word before your tries run out!

## Demo

```
Welcome to Word Guess!
The word has 6 letters. You have 6 wrong guesses allowed.

_ _ _ _ _ _
Tries left: 6
Guess a letter: p
Correct!

p _ _ _ _ _
Tries left: 6
Guess a letter: z
Wrong guess.
...
```

## Getting Started

### Prerequisites

- Python 3.x installed

### Run the game

```bash
python3 word_guess.py
```

## Features

- Clean, single-file implementation (~70 lines)
- Input validation (rejects non-letters, repeated guesses)
- Replay option after each round
- Easy to extend with your own word list

## Customize

Want a different theme (movies, countries, tech terms)? Just edit the `WORDS`
list at the top of `word_guess.py`:

```python
WORDS = [
    "python", "developer", "keyboard", ...
]
```

You can also change the difficulty by adjusting `MAX_TRIES`.

## Project Structure

```
word-guess/
├── word_guess.py   # Game logic
└── README.md       # This file
```

## License

Free to use and modify for personal or educational purposes.
