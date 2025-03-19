# Asteroids Game

A classic Asteroids arcade game implemented in Python using Pygame.

## Overview

This is a simple implementation of the classic Asteroids arcade game. Control a spaceship, shoot asteroids, and try to survive as long as possible without colliding with any asteroids.

## Features

- Player-controlled spaceship with rotation and movement
- Randomly spawning asteroids that enter from the edges of the screen
- Shooting mechanics to destroy asteroids
- Collision detection between the player, asteroids, and shots
- Asteroids split into smaller pieces when hit

## Requirements

- Python 3.x
- Pygame 2.6.1

## Installation

1. Make sure you have Python installed on your system
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## How to Play

1. Run the game:
   ```
   python main.py
   ```

2. Controls:
   - `W` - Move forward
   - `S` - Move backward
   - `A` - Rotate counter-clockwise
   - `D` - Rotate clockwise
   - `SPACE` - Shoot

3. Objective:
   - Destroy asteroids by shooting them
   - Avoid colliding with asteroids
   - Survive as long as possible

4. Game Mechanics:
   - Asteroids spawn from the edges of the screen at random intervals
   - When hit, larger asteroids split into two smaller asteroids
   - The game ends if your ship collides with an asteroid

## Project Structure

- `main.py`: The main game loop and initialization
- `constants.py`: Game constants and configuration values
- `circleshape.py`: Base class for circular game objects (player, asteroids, shots)
- `player.py`: Player ship implementation
- `asteroid.py`: Asteroid implementation
- `asteroidfield.py`: Handles spawning of asteroids
- `shot.py`: Player projectile implementation

## Game Constants

You can modify the game by changing values in `constants.py`:

- Screen dimensions: `SCREEN_WIDTH`, `SCREEN_HEIGHT`
- Asteroid properties: `ASTEROID_MIN_RADIUS`, `ASTEROID_KINDS`, `ASTEROID_SPAWN_RATE`
- Player properties: `PLAYER_RADIUS`, `PLAYER_TURN_SPEED`, `PLAYER_SPEED`, `PLAYER_SHOOT_SPEED`, `PLAYER_SHOOT_COOLDOWN`
- Shot properties: `SHOT_RADIUS`

## Known Issues and Limitations

1. Asteroids and player ship can move off-screen with no wraparound
2. No scoring system implemented
3. No game reset functionality after game over
4. No visual or audio effects for collisions or shots

## Future Enhancements

Potential improvements for the game:

1. Add score tracking and display
2. Implement screen wrapping for the player and asteroids
3. Add visual effects (explosions, particle effects)
4. Add sound effects and background music
5. Add game states (menu, game over screen, etc.)
6. Add power-ups or multiple weapon types
7. Add enemy ships that shoot at the player

## License

This project is open source and available for educational purposes.

## Credits

This implementation of Asteroids was created using Python and Pygame.
