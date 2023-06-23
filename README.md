
# The Worst Chess Game Ever ♟️

Welcome to The Worst Chess Game Ever! This project brings you an intentionally terrible chess game that can be played mathematically. 🎉🙈


## Overview

This project aims to create a hilarious and challenging chess play that will blow your mind by its stupidity. With Python 3.10.6, Stockfish as the chess engine, and the "chess" library for Python, we have created a game that will surely frustrate even the most experienced chess players. 🤯🔀
## Features

- **Horrendous AI**: The AI in this game is intentionally designed to make the worst possible moves, leading to unpredictable and nonsensical gameplay. Expect the unexpected! 😱
- **Mathematical Approach**: Instead of relying on human-like decision-making, our game uses mathematical calculations to determine moves, resulting in a truly unique and mind-boggling chess experience. 🔢🧠
- **Stockfish Integration**: We have integrated the powerful Stockfish chess engine to assist with move calculations. Even though this AI is powerful, it is equally powerful the other way, creating the worst moves possible. 🐟🤦‍♂️
## Requirements

- **Python 3.10.6**: The game is developed using Python 3.10.6. Make sure you have it installed on your system.
- **Stockfish**: The Stockfish chess engine is a crucial component of this project. Please follow the installation instructions for your operating system: Stockfish GitHub Repository.
`pip install stockfish`
- **"chess"** Library: We utilize the "chess" library for Python, which provides useful functionalities for chess-related operations. Install it by running the following command:
 `pip install chess`
# How it is done? ♟️

The main idea behind this project is to abuse `move = stockfish.get_top_moves(n)` function that returns N first moves of **Stockfish** evaluation. So, we should take a bigger value of those possible moves. For e.g.: `worst_move = stockfish.get_top_moves(60)`. Now, we should understand, that this func. returns a dictionary of moves. So, we could extract the last move from this list. So, this line looks like this: `worst_move = stockfish.get_top_moves(60)[-1]`

I could increase the N value of this func. but this is not so necessary in my opinion. 60 wil be enough.

# Eval bar 🤯

[alt text](https://github.com/plugg1N/worst-chess-game/blob/main/eval.jpg?raw=true)
