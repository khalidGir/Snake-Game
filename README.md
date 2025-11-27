# Snake Game

A classic Snake game implementation using HTML5 Canvas, JavaScript, and CSS. Guide the snake to eat food and grow while avoiding collisions with walls and itself.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [How to Play](#how-to-play)
- [Game Rules](#game-rules)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Code Overview](#code-overview)
- [Customization](#customization)
- [License](#license)

## Demo

![Snake Game Demo](demo.gif)

> Note: You need to create a demo.gif if you want to show an actual demo.

## Features

- Classic Snake gameplay
- Score tracking
- Responsive design
- Modern UI with glowing effects
- Game over screen with restart option
- Keyboard controls (arrow keys)
- Collision detection (walls and self)

## Technologies Used

- HTML5 Canvas
- CSS3 (with gradients and shadows)
- Vanilla JavaScript (ES6+)
- Responsive design principles

## How to Play

1. Open `snake.html` in your web browser
2. Use the arrow keys to control the snake's direction:
   - ↑ (Up Arrow): Move up
   - ↓ (Down Arrow): Move down
   - ← (Left Arrow): Move left
   - → (Right Arrow): Move right
3. Guide the snake to eat the food (magenta squares)
4. Each food item increases your score by 1 point
5. Avoid hitting the walls or the snake's own body
6. When game is over, click "Restart" to play again

## Game Rules

- The snake grows each time it eats food
- Game ends if the snake hits the wall or itself
- The snake cannot reverse its direction (e.g., if moving right, it cannot move left)
- Player's score increases by 1 for each food eaten

## Installation

1. Clone or download this repository
2. Open `snake.html` in your web browser

Alternatively, you can run a local server:

### Using Python

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then open `http://localhost:8000/snake.html` in your browser.

### Using Node.js

If you have Node.js installed, you can use `http-server`:

```bash
npm install -g http-server
http-server
```

Then open `http://localhost:8080/snake.html` in your browser.

## Project Structure

```
snake-game/
├── snake.html     # Main HTML file containing game structure and logic
├── snake.css      # Stylesheet for the game UI
└── README.md      # This file
```

## Code Overview

### HTML (`snake.html`)

- Contains a canvas element for rendering the game
- Displays the player's score
- Shows game over screen with restart button
- Includes all game logic in JavaScript

### CSS (`snake.css`)

- Modern dark gradient background
- Glowing effects for snake and food
- Responsive design for different screen sizes
- Styling for game over overlay and restart button

### JavaScript (within `snake.html`)

- Game state management (snake position, direction, food position)
- Rendering functions for snake and food
- Collision detection
- Keyboard input handling
- Score tracking
- Game loop with timed updates

## Customization

You can easily customize the game by modifying the following values in `snake.html`:

- Game speed: Adjust the timeout value in `setTimeout(gameLoop, 100)` - lower is faster
- Grid size: Change the `gridSize` variable
- Colors: Modify the `fillStyle` and `shadowColor` values in the drawing functions
- Initial snake position: Edit the initial values in the `snake` array

To change styles like colors, fonts, or sizes, modify `snake.css`.

## License

This project is open source and available under the [MIT License](LICENSE).

Feel free to use, modify, and distribute this code for personal or educational purposes.