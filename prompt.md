# Pac-Man Game Development Prompt

Create a fully functional Pac-Man game using HTML, CSS, and JavaScript. The game should be contained in a single HTML file with embedded CSS and JavaScript.

## Core Requirements

### Game Board
- Create a 19x21 grid maze (classic Pac-Man dimensions)
- Use a 2D array to represent the maze layout with different cell types:
  - 0: Empty space
  - 1: Wall
  - 2: Dot (small pellet)
  - 3: Power pellet (large pellet)
  - 4: Ghost spawn area
- Implement the classic Pac-Man maze design or create a simplified version
- Render the maze using HTML Canvas or CSS Grid

### Pac-Man Character
- Yellow circular character that can move in 4 directions (up, down, left, right)
- Smooth movement between grid cells (not instant teleportation)
- Mouth animation that opens/closes while moving
- Directional facing based on movement direction
- Wraparound movement on horizontal edges of the screen
- Collision detection with walls (cannot move through them)

### Ghosts
- Implement 4 ghosts with different colors (red, pink, cyan, orange)
- Each ghost should have basic AI movement patterns
- Ghosts should avoid walls and move through the maze
- Normal state: Chase Pac-Man or move randomly
- Frightened state: Move away from Pac-Man (when power pellet eaten)
- Return to spawn after being eaten

### Game Mechanics
- Pac-Man eats dots by moving over them (remove from board, increase score)
- Power pellets make ghosts vulnerable for a limited time
- Eating frightened ghosts gives bonus points and sends them back to spawn
- Game over when Pac-Man collides with a non-frightened ghost
- Level complete when all dots are collected
- Score system: dots = 10 points, power pellets = 50 points, ghosts = 200/400/800/1600 points

### Controls
- Arrow keys or WASD for movement
- Smooth, responsive controls
- Queue next direction if current direction is blocked

### UI Elements
- Score display
- Lives counter (start with 3 lives)
- Game over screen
- Start/restart functionality
- Simple start screen

## Technical Implementation

### File Structure
- Single HTML file containing:
  - HTML structure for game container and UI
  - CSS for styling and animations
  - JavaScript for all game logic

### Performance Considerations
- Use requestAnimationFrame for smooth animations
- Efficient collision detection
- Optimize rendering to avoid unnecessary redraws

### Code Organization
```javascript
// Suggested class structure:
class Game {
  // Main game controller
}

class Pacman {
  // Pac-Man character logic
}

class Ghost {
  // Individual ghost behavior
}

class Maze {
  // Maze rendering and collision detection
}
```

## Bonus Features (if time permits)
- Sound effects for eating dots, power pellets, and ghosts
- Fruit bonus items that appear occasionally
- Multiple levels with increasing difficulty
- High score persistence using localStorage
- Mobile touch controls
- Particle effects for eating pellets

## Visual Style
- Retro arcade aesthetic with bright colors
- Black background for the maze
- Blue walls, yellow dots, larger power pellets
- Classic Pac-Man yellow with simple animation
- Colorful ghosts with simple eye details

## Testing Requirements
- Game should run smoothly at 60 FPS
- All collision detection should work accurately
- Ghost AI should be challenging but fair
- Controls should be responsive
- Game state should reset properly on restart

Please create a complete, playable Pac-Man game that captures the essence of the original while being implementable in a single HTML file. Focus on core gameplay mechanics first, then add polish and bonus features.