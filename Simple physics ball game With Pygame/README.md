# Simple Physics Ball Game (Pygame)

A playful 2D physics sandbox built with Pygame. Add colorful balls, watch them bounce under gravity, and see realistic ball–ball collisions in real time. Includes a handy sidebar with buttons for quick interactions.

## Features

- Real-time physics with gravity and wall bounces
- Realistic ball–ball collisions with mass and restitution
- Add 1 or 5 random balls with a click
- Clear all balls instantly
- Keyboard boost (give all balls an upward push)
- 60 FPS rendering with a simple sidebar UI

## Requirements

- Python 3.x
- Jupyter Notebook
- `pygame`

Install dependencies:
```bash
pip install pygame
```

## Usage

1. Open `physics_ball_game.ipynb` in Jupyter Notebook.
2. Run all cells to launch the game window.
3. Interact using the controls below.

## Controls

- Sidebar buttons:
  - "+ Add Random Ball" — add one ball
  - "+ Add 5 Balls" — add five balls
  - "Clear Balls" — remove all balls
- Keyboard:
  - SPACE — boost all balls upward
  - ESC — quit
- You can also close the window via the window close button.

## Tweaks

- Adjust gravity and bounce behavior near the top of the notebook:
  - `gravity`
  - `bounce_factor`
- Game and sidebar sizes are defined by `GAME_WIDTH`, `HEIGHT`, and `SIDEBAR_WIDTH`.

---

Have fun tinkering with 2D physics!
