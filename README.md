# Ping Pong Game

This is a simple Ping Pong game created using Python and Turtle graphics library.

## Installation

1. Make sure you have Python installed on your system. You can download it from [here](https://www.python.org/downloads/).
2. Clone this repository to your local machine or download the ZIP file and extract it.

## Usage

1. Open a terminal or command prompt.
2. Navigate to the directory where the game files are located.
3. Run the following command to start the game:
```bash
python main.py
```
4. Use the following controls to play the game:
* Right Paddle: Up and Down arrow keys
* Left Paddle: W (up) and S (down) keys
* Try to hit the ball with your paddle to keep the game going. If the ball passes your paddle, your opponent gets a point.

## Dependencies
- Python 3.x
- Turtle graphics library (usually comes pre-installed with Python)

# Ping Pong Game - Documentation

This document provides an overview of the methods available in the Python files `ball.py`, `scoreboard.py`, and `paddle.py`, which are used in the Ping Pong game.

## ball.py

### Methods

#### `__init__(self)`

- Initializes a new instance of the `Ball` class.
- Sets up the attributes of the ball such as color, shape, initial movement speed, and direction.

#### `move(self)`

- Moves the ball by updating its position based on its current x and y coordinates and the movement increments (`x_move` and `y_move`).

#### `bounce_y(self)`

- Inverts the direction of the ball's vertical movement (`y_move`) when it hits the top or bottom border of the screen.

#### `bounce_x(self)`

- Inverts the direction of the ball's horizontal movement (`x_move`) when it collides with a paddle.
- Also decreases the movement speed of the ball.

#### `reset_position(self)`

- Resets the position of the ball to the center of the screen.
- Resets the movement speed and adjusts the direction of the ball horizontally.

## scoreboard.py

### Methods

#### `__init__(self)`

- Initializes a new instance of the `Scoreboard` class.
- Sets up attributes such as color, position, and initial scores for both players.

#### `update_scoreboard(self)`

- Clears the current scoreboard display.
- Writes the updated scores for both players on the screen.

#### `l_point(self)`

- Increases the left player's score by 1.
- Updates the scoreboard display accordingly.

#### `r_point(self)`

- Increases the right player's score by 1.
- Updates the scoreboard display accordingly.

## paddle.py

### Methods

#### `__init__(self, position)`

- Initializes a new instance of the `Paddle` class.
- Sets up attributes such as shape, color, size, and position of the paddle.

#### `go_up(self)`

- Moves the paddle upwards by adjusting its y-coordinate upwards.

#### `go_down(self)`

- Moves the paddle downwards by adjusting its y-coordinate downwards.

