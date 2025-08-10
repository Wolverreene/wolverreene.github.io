---
layout: page
title: 2D Space Shooter Game
description: A 2D space shooter game where a player controls a spaceship to shoot down enemies and earn points. It was developed using OOP concepts and techniques in Python.
img: assets/img/mine/2d-game.png
importance: 1
category: fun
---

# 2D Space Shooter Game

This is a 2D space shooter game where the player controls a spaceship to shoot down enemies and earn points. The game is built using Object-Oriented Programming (OOP) principles in Python, utilizing the Pygame library for graphics and interaction.

## Features

- **Player Controls**: Use the left and right arrow keys to move the spaceship, and the spacebar to shoot bullets.
- **Enemies**: Enemies spawn from the top of the screen and move downward.
- **Collisions**: When the player's bullets collide with enemies, the enemies are destroyed and the player's score increases.
- **High Scores**: The game tracks high scores using an SQLite database.
- **Game Over**: When the player collides with an enemy, the game ends and displays the "Game Over" message.
- **Interactive Database**: Player names and scores are saved to a database, and the top scores are displayed at the end of each game.

## Game Design

The game uses several classes to handle different aspects of the game:

- **Database Class**: Manages interactions with the SQLite database, storing and retrieving high scores.
- **Player Class**: Handles the player's movement, shooting, and score management.
- **Bullet Class**: Manages the behavior of the player's bullets.
- **Enemy Class**: Controls enemy movement, spawning, and collision detection.
- **ScoreCounter Class**: Displays the player's current score on the screen.

The game loop ensures continuous updating of the game state, including player input handling, enemy movement, bullet updates, and collision checks. It also ensures the proper display of game elements.

## Requirements

- Python 3.x
- Pygame library
- SQLite (for high score management)

You can install the required dependencies with:

```bash
pip install pygame sqlite3
```

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/2D_SpaceShooterGame.git
cd 2D_SpaceShooterGame
```

## Usage

Run the game by executing:

```bash
python space_shooter_game.py
```

The game will open in a window with a size of 800x600 pixels. Use the arrow keys to move the spaceship and spacebar to shoot.

## Demo

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/video/2D-Game.mp4" title="example image" %}
    </div>
</div>
<div class="caption">
    A demo video showing the gameplay and code implementation.
</div>

## Documentation

Apart from the game itself, I have also created a complete documentation that outlines the game's design, implementation, test plan, optimization logs, and review discussions. The documentation is available in the [**2D-GameDoc.pdf**](assets/pdf/2D-GameDoc.pdf) file in the repository.
