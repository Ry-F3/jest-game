# Jest Simon Game

Welcome to the Jest Simon Game! This is a simple implementation of the classic Simon memory game built with HTML, CSS, and JavaScript.

## Live Demo

You can see a live demo of the game at the following link:

[Play Simon Game](https://ry-f3.github.io/jest-game/)

## Game Overview

The Jest Simon Game challenges players to remember and replicate increasingly complex sequences of button presses. Players are required to follow a sequence of lights, and if they make a mistake, the game resets.

## Features

- **Memory Challenge**: The game displays a sequence of lights that the player must replicate.
- **Score Tracking**: The player's score increases with each successful sequence.
- **New Game**: Start a fresh game anytime with the "New Game" button.
- **Visual Feedback**: Buttons light up when it's their turn in the sequence.

## How to Play

1. **Start a New Game**: Click the "New Game" button to begin a new session.
2. **Follow the Sequence**: Observe the sequence of lights as they light up.
3. **Replicate the Sequence**: Click on the buttons in the same order as shown.
4. **Score**: Your score increases with each correct sequence. Incorrect moves will reset the game.

## Installation and Setup

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/jest-simon-game.git


## Code Overview

The game logic is implemented in JavaScript and consists of several key functions and a game state object. Below is a detailed explanation of each part of the code.

### Game State Object

```javascript
let game = {
    currentGame: [],
    playerMoves: [],
    score: 0,
    turnNumber: 0,
    lastButton: "",
    turnInProgress: false,
    choices: ["button1", "button2", "button3", "button4"]
};


## Game Object

The `game` object stores the state and configuration of the game:

- `currentGame`: An array that stores the sequence of button IDs for the current game.
- `playerMoves`: An array that tracks the player’s button presses.
- `score`: The player’s score, which increments with each correct sequence.
- `turnNumber`: The current turn in the game.
- `lastButton`: The ID of the last button pressed by the player.
- `turnInProgress`: A boolean flag indicating if a turn is currently being played.
- `choices`: An array of button IDs used in the game.