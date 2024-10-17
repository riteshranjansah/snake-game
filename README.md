# Snake Game

This is a simple and classic Snake Game implemented using **Pygame**. The player controls a snake that grows longer as it eats fruit, and the game ends if the snake runs into itself or the boundaries.

## Features

- **Snake Movement**: The player can control the snake using the arrow keys (Up, Down, Left, Right).
- **Snake Growth**: Each time the snake eats the fruit, it grows longer.
- **Game Over**: The game ends when the snake collides with the screen boundaries or with itself.
- **Score Display**: The score is displayed in the top-right corner based on the number of fruit eaten.
- **Sound Effects**: The game features a crunch sound effect when the snake eats the fruit.

## Technologies Used

- **Python**: The programming language used to implement the game logic.
- **Pygame**: A library for creating video games in Python. It provides tools for handling graphics, sounds, and user input.
- **Vector2**: Used for snake movement and position tracking.
- **Graphics & Sound**: Custom graphics and sound effects to enhance the game experience.

## Installation

### Prerequisites

- **Python**: Make sure you have Python 3.x installed. You can download it from [python.org](https://www.python.org/downloads/).
- **Pygame**: Install the Pygame library using pip:

```bash
pip install pygame
```

### Download the Game

1. Clone the repository:

```bash
git clone https://github.com/riteshranjansah/snake-game.git
```

2. Navigate into the project directory:

```bash
cd snake-game
```

3. Run the game:

```bash
python snake.py
```

### Game Assets

The game uses the following assets located in the `Graphics/` and `Sound/` folders:
- **Graphics**: Images for the snake, fruit, and background tiles.
- **Sound**: A sound effect for when the snake eats the fruit (`crunch.wav`).

Ensure these assets are available in the respective folders or you can modify the paths in the script accordingly.

## How to Play

- **Controls**: Use the arrow keys on your keyboard to move the snake:
  - **Up Arrow**: Move the snake up
  - **Down Arrow**: Move the snake down
  - **Left Arrow**: Move the snake left
  - **Right Arrow**: Move the snake right

- **Objective**: Eat the apple (fruit) that appears randomly on the screen. Each time you eat an apple, the snake grows longer.
- **Game Over**: The game will end if:
  - The snake runs into the boundary (the edge of the screen).
  - The snake runs into itself.

- **Score**: The score is displayed in the top-right corner and increases with each fruit eaten. The score represents the length of the snake minus the initial length (3 blocks).

## Game Logic

### Snake Class

The `SNAKE` class represents the snake and handles:
- **Snake Movement**: The snake moves continuously in the direction set by the user.
- **Snake Growth**: When the snake eats an apple, a new block is added to the snake's body.
- **Collision Detection**: Detects if the snake collides with the screen boundaries or itself, triggering the game over.

### Fruit Class

The `FRUIT` class represents the fruit that the snake eats:
- The fruit randomly appears at different positions on the grid.
- When the snake eats the fruit, the fruit is randomized again and placed in a new position.

### Main Class

The `MAIN` class manages the overall game:
- It controls the main game loop, updates the snake's position, checks for collisions, and handles drawing the game elements on the screen.

## Directory Structure

```
snake-game/
│
├── Graphics/
│   ├── head_up.png          # Snake head facing up
│   ├── head_down.png        # Snake head facing down
│   ├── head_right.png       # Snake head facing right
│   ├── head_left.png        # Snake head facing left
│   ├── tail_up.png          # Snake tail facing up
│   ├── tail_down.png        # Snake tail facing down
│   ├── tail_right.png       # Snake tail facing right
│   ├── tail_left.png        # Snake tail facing left
│   ├── body_vertical.png    # Snake body (vertical)
│   ├── body_horizontal.png  # Snake body (horizontal)
│   ├── body_tr.png          # Snake body (top-right corner)
│   ├── body_tl.png          # Snake body (top-left corner)
│   ├── body_br.png          # Snake body (bottom-right corner)
│   ├── body_bl.png          # Snake body (bottom-left corner)
│   ├── apple.png            # The fruit (apple)
│
├── Sound/
│   ├── crunch.wav           # Sound effect when the snake eats a fruit
│
├── Font/
│   ├── PoetsenOne-Regular.ttf  # Font used for displaying the score
│
├── snake.py                 # Main game logic script
└── README.md                # This file
```

## Contributing

Feel free to contribute to this project. If you want to improve it, you can:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request on GitHub.

## License

This project is just a fun, open-source game for demonstration purposes. No license has been applied to this repository, so feel free to use, modify, and distribute it as you like.
