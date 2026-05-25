# PlaneGamePython
<img width="801" height="632" alt="image" src="https://github.com/user-attachments/assets/f6df72d8-3500-45f1-a9f4-c1f47307d8ce" />
# Jet Dodger

A simple 2D arcade game built with **Python** and **Pygame**. The player controls a jet, dodges incoming missiles, and flies through a scrolling sky with clouds.

## Demo

The game opens an 800×600 window where:

- The player jet can move up, down, left, and right.
- Missiles spawn from the right side of the screen and move left.
- Clouds scroll across the background.
- The game ends when the jet collides with a missile.
- Pressing `Esc` closes the game.

## Features

- Sprite-based player, enemy, and cloud objects
- Random enemy spawn positions and speeds
- Collision detection between the player and missiles
- Screen boundary checks to keep the player visible
- Timed spawning for enemies and clouds
- 30 FPS game loop
- Optional commented-out sound and music support

## Requirements

- Python 3.8+
- Pygame

Install Pygame with:

```bash
pip install pygame
```

## Project Structure

```text
.
├── main.py
├── jet.png
├── missile.png
├── cloud.png
└── README.md
```

> Note: The Python file can be named anything, but this README assumes it is saved as `main.py`.

## Required Assets

The game expects the following image files to be in the same folder as the Python script:

- `jet.png` — player sprite
- `missile.png` — enemy missile sprite
- `cloud.png` — cloud sprite

Optional audio files are referenced in the code but currently commented out:

- `Apoxode_-_Electric_1.mp3`
- `Rising_putter.ogg`
- `Falling_putter.ogg`
- `Collision.ogg`


## Controls

| Key | Action |
| --- | --- |
| Up Arrow | Move up |
| Down Arrow | Move down |
| Left Arrow | Move left |
| Right Arrow | Move right |
| Esc | Quit game |

## Gameplay

Your goal is to avoid the incoming missiles for as long as possible. Missiles appear from the right side of the screen at random heights and move toward the left at random speeds. If a missile collides with the jet, the game ends.

## Customization Ideas

You can expand the game by adding:

- A score counter
- Lives or health points
- Increasing difficulty over time
- A start menu and game-over screen
- Sound effects and background music
- Different enemy types
- Power-ups

## Notes

The current code uses local image files with `pygame.image.load()`, so the game must be run from the folder containing the sprite assets. If assets are missing or named differently, Pygame will raise a file loading error.

## License

This project is open source. Add your preferred license before publishing, such as MIT, Apache-2.0, or GPL-3.0.
