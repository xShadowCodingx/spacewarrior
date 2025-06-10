# Space Warrior

A modern browser-based space shooter game built with HTML5 Canvas and JavaScript using the Cursor Editor to assist with function and README generation.

## Game Overview

Space Warrior is an engaging space shooter where players control a spaceship to defend against waves of enemy ships. The game features smooth controls, multiple enemy types, power-ups, and an engaging scoring system.

## Features

- Responsive canvas-based gameplay
- Multiple enemy types with different behaviors
- Mouse and touch controls
- Score tracking system
- Health management
- Pause functionality
- Game over handling
- Sound effects and background music
- Mobile-friendly design

## Technical Architecture

### Core Components

#### Game Class
The main game controller that manages the game loop, state, and all game elements.

Key methods:
- `constructor()`: Initializes game canvas, state, and event listeners
- `startGame()`: Begins the game session
- `update()`: Handles game logic updates
- `draw()`: Renders all game elements
- `gameLoop()`: Main game loop using requestAnimationFrame
- `checkCollisions()`: Manages collision detection between game objects

#### Player Class
Controls the player's spaceship with the following features:
- Mouse/touch-based movement
- Shooting mechanics
- Health management

#### Enemy System
Three types of enemies with different behaviors:
- Green Enemies (60% spawn rate)
- Blue Enemies (25% spawn rate)
- Red Enemies (15% spawn rate)

Each enemy type has unique:
- Health points
- Movement patterns
- Shooting behavior
- Point values

#### Projectile System
- Player projectiles
- Enemy projectiles
- Collision detection
- Screen boundary checking

#### UI Elements
- Score display
- Health indicator
- Pause menu
- Game over modal
- Start menu

## Controls

- **Movement**: Mouse or touch controls
- **Shooting**: Click or tap
- **Pause**: ESC key or pause button
- **Menu Navigation**: Click/tap on menu items

## Game States

1. **Menu State**: Initial game screen
2. **Playing State**: Active gameplay
3. **Paused State**: Game temporarily halted
4. **Game Over State**: End of game session

## Technical Implementation

### Canvas Management
- Responsive canvas sizing
- Automatic window resize handling
- High-performance rendering

### Event System
- Mouse movement tracking
- Touch event support
- Keyboard controls
- Window resize handling

### Collision Detection
- Rectangle-based collision system
- Efficient collision checking between:
  - Player projectiles and enemies
  - Enemy projectiles and player
  - Enemies and player

### Audio System
- Background music
- Sound effects for:
  - Shooting
  - Explosions
  - Game over
  - Enemy lasers

## Performance Considerations

- Efficient object pooling for projectiles and explosions
- Canvas optimization techniques
- Frame-rate independent movement
- Memory management through proper cleanup

## Browser Compatibility

The game is compatible with modern browsers that support:
- HTML5 Canvas
- ES6 JavaScript
- Touch events
- Audio API

## Getting Started

1. Play the game online: [Space Warrior](https://www.shadowcoding.com/projects/web-games/space-warrior/game.html)
2. Clone the repository
3. Open `game.html` in a modern web browser
4. Click "Start Game" to begin playing

## Development

To modify or enhance the game:

1. Edit the game logic in `game.js`
2. Modify enemy behaviors in the Enemy class
3. Adjust game parameters in the Game class
4. Update UI elements in the HTML file

## License

Open Source - Help yourself to forking, copying, or anything else.

## Credits

### Audio Assets
- **Explosion Sound**: TinyWorlds - [OpenGameArt](https://opengameart.org/content/explosion-0)
- **Enemy Laser Sound**: Mobeyee Sounds (mobeyee.com) - [OpenGameArt](https://opengameart.org/content/laser-shot-0)
- **Player Laser Sound**: dklon - [OpenGameArt](https://opengameart.org/content/laser-fire)
- **Background Music**: Nia Mi - [OpenGameArt](https://opengameart.org/content/fun-background)
- **Game Over Sound**: CleytonKauffman - [OpenGameArt](https://opengameart.org/content/game-over-theme-ii)

### Visual Assets
- **Player Spaceship**: Skorpio - [OpenGameArt](https://opengameart.org/content/spaceship-6)
- **Enemy Spaceships**: 
  - Red Enemy: Skorpio - [OpenGameArt](https://opengameart.org/content/spaceship-4)
  - Blue & Green Enemies: Skorpio - [OpenGameArt](https://opengameart.org/content/spaceship-8)
- **Explosion Animation**: Master484 - [OpenGameArt](https://opengameart.org/content/explosion-set-1-m484-games)
- **Sound Control Icons**: oglsdl - [OpenGameArt](https://opengameart.org/content/sound-on-sound-off)

All assets are used under the OpenGameArt license. Special thanks to all the talented artists and creators who made these assets available for use. 
