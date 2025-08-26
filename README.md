# Pathfinding Game

A 2D maze game where you collect points while avoiding two AI enemies that use different pathfinding algorithms.

## Features
- **Two intelligent enemies** using BASIC (A*) and GREEDY pathfinding
- **Temporary obstacles** - drop barriers with spacebar to block enemies
- **Path visualization** - see enemy routes in real-time
- **Point collection** system with automatic respawn

## Controls
- **Arrow keys:** Move player
- **Spacebar:** Drop temporary obstacle (5s duration, 10s cooldown)

## Technology
- **Language:** C++ with SFML
- **Map:** Fixed 30x20 tile labyrinth
- **Graphics:** 32px tiles, 60 FPS

## Required Files
### Assets folder:
- `floor.png`, `wall2.png` - Map tiles
- `player2.png`, `enemy2.png` - Character sprites  
- `path.png`, `este.png`, `piste.png` - Game objects

### Headers:
- `sfml_view.h` - View functions
- `enemy_agent.h` - AI logic
- `point_ball.h` - Point system

## Game Mechanics
- **Enemies** update every 15 frames, recalculate paths around obstacles
- **Player** has movement delay (0.15s) to prevent spam
- **Collision** with enemies ends the game
- **Points** collected by walking over point balls

## Build Requirements
- SFML library installed
- All texture files in `assets/` folder
- Header dependencies in project directory