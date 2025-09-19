# ASCII 3D Room

A retro-style 3D room rendered entirely in ASCII characters using raycasting techniques similar to classic games like Doom and Wolfenstein 3D.

## 🎮 [Play Online](https://yourusername.github.io/ascii-3d-room)

## Features

- **Full 3D Raycasting**: Navigate a 3D environment rendered in ASCII
- **Smooth Movement**: WASD controls with diagonal movement normalization
- **Look Around**: Arrow keys for pitch and yaw rotation
- **Collision Detection**: Realistic wall collision with sliding mechanics
- **Floor Perspective**: Converging grid lines create proper depth perception
- **Interactive Objects**: 3D sprites with distance-based level of detail
- **Performance Optimized**: Runs at 30+ FPS in modern browsers

## Controls

- **WASD**: Move around
- **Arrow Keys**: Look around (up/down/left/right)
- **Esc**: Pause/Resume
- **?**: Toggle help screen
- **F1**: Toggle debug information

## Technical Details

- **Resolution**: 120×40 ASCII character grid
- **Field of View**: 66 degrees
- **Rendering**: DDA raycasting algorithm with fisheye correction
- **ASCII Palette**: `@#%*=+:-.` for distance-based shading
- **Physics**: Circular collision detection with 0.3 unit radius
- **Performance**: RequestAnimationFrame loop with FPS monitoring

## Browser Compatibility

Works in all modern desktop browsers:
- Chrome/Chromium
- Firefox
- Safari
- Edge

## Implementation

Built with vanilla JavaScript, HTML5, and CSS3. No external dependencies required.

---

*Created as a demonstration of ASCII-based 3D rendering techniques*