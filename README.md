# 🦕 Chrome Dino 3D - Endless Runner

A thrilling 3D endless runner game featuring a dinosaur navigating through a procedurally generated prehistoric landscape!

## 🎮 Game Features

### Core Gameplay
- **Third-person 3D perspective** - Camera positioned behind and above the dinosaur
- **Automatic forward movement** - The dinosaur runs forward continuously
- **Procedural terrain generation** - Dynamic hills, rocks, and natural features
- **Multiple obstacle types**:
  - 🪨 **Rocks** - Jump over them
  - 🕳️ **Pits** - Jump across them
  - 🐦 **Flying Birds** - Duck under them
  - 🚪 **Gates** - Duck under the crossbar

### Controls
- **SPACE** - Jump (avoid ground obstacles)
- **DOWN ARROW** - Duck (avoid overhead obstacles)

### Visual Style
- Low-poly 3D graphics with stylized aesthetic
- Dynamic lighting and shadows
- Beautiful sky environment with sunset atmosphere
- Smooth animations and particle effects

### Scoring System
- **Distance Counter** - Track how far you've traveled
- **Obstacles Avoided** - Count successful obstacle navigation  
- **High Score** - Persistent best distance record
- **Progressive Difficulty** - Speed increases over time

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start the development server:**
   ```bash
   npm start
   ```

3. **Open your browser and navigate to:**
   ```
   http://localhost:3000
   ```

### Building for Production

```bash
npm run build
```

## 🎯 How to Play

1. **Click "START ADVENTURE"** to begin
2. **Use SPACE** to jump over rocks and pits
3. **Use DOWN ARROW** to duck under birds and gates
4. **Survive as long as possible** while the speed increases
5. **Beat your high score!**

### Tips for High Scores
- ⏱️ **Timing is crucial** - Jump and duck at the right moment
- 👀 **Look ahead** - Anticipate upcoming obstacles
- 🏃 **Stay in rhythm** - Find your timing pattern
- 🎯 **Practice makes perfect** - Each run teaches you the patterns

## 🛠️ Technology Stack

- **React** - UI framework
- **Three.js** - 3D graphics and rendering
- **@react-three/fiber** - React renderer for Three.js
- **@react-three/drei** - Useful helpers and abstractions
- **@react-three/cannon** - Physics engine for collision detection
- **cannon-es** - Physics simulation

## 🏗️ Project Structure

```
src/
├── components/
│   ├── Game.js          # Main game component and loop
│   ├── Dinosaur.js      # Player character with physics
│   ├── Terrain.js       # Procedural landscape generation
│   ├── ObstacleManager.js # Obstacle spawning and management
│   └── Camera.js        # Third-person camera system
├── App.js               # Root component with game states
├── index.js             # Application entry point
└── index.css            # Global styles and UI
```

## 🎨 Game Mechanics

### Dinosaur Physics
- Realistic jumping physics with gravity
- Collision detection for obstacles
- Ducking animation with hitbox adjustment
- Running animation with subtle movement

### Procedural Generation
- **Terrain Segments** - Infinite scrolling landscape
- **Random Hills** - Varying heights and positions  
- **Decorative Elements** - Rocks and natural features
- **Dynamic Obstacles** - Spawned based on difficulty

### Progressive Difficulty
- Speed increases every 500 meters
- More frequent obstacle spawning
- Larger obstacles at higher difficulties
- Mixed obstacle types for variety

## 🔧 Customization

### Adjusting Difficulty
Edit `ObstacleManager.js` to modify:
- Spawn frequency: `spawnDistance` calculation
- Obstacle types: `types` array and `weights`
- Obstacle sizes: `scale` property

### Visual Modifications
Edit component files to adjust:
- **Colors**: Change `meshLambertMaterial color` properties
- **Lighting**: Modify `directionalLight` and `ambientLight`
- **Terrain**: Adjust hill and rock generation in `Terrain.js`

### Controls
Modify `Dinosaur.js` `handleKeyDown` function to change:
- Jump key (currently SPACE)
- Duck key (currently ArrowDown)
- Add new abilities

## 🐛 Troubleshooting

### Common Issues
- **Game not loading**: Ensure all dependencies are installed
- **Poor performance**: Try reducing obstacle count or terrain complexity
- **Controls not working**: Make sure the game window has focus

### Performance Optimization
- The game automatically adjusts based on device capabilities
- Physics calculations are optimized for smooth 60fps gameplay
- Terrain segments are efficiently recycled

## 🎵 Future Enhancements

Potential features to add:
- 🎵 **Sound effects and music**
- 🌅 **Day/night cycle**
- ⛅ **Weather effects**
- ⚡ **Power-ups** (speed boost, shield, etc.)
- 🏆 **Achievement system**
- 🎨 **Character customization**
- 📱 **Mobile touch controls**

## 📄 License

This project is open source and available under the MIT License.

---

**Have fun running with the dinosaur! 🦕💨**
