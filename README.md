# ASCII 3D Forest

An immersive ASCII-based 3D forest environment using advanced raycasting techniques. Walk through a procedurally generated forest with realistic tree collision, atmospheric effects, and dynamic lighting.

## 🎮 [Play Online](https://a-false-god.github.io/asci/)

## Features

### 🌲 **Forest Environment**
- **Procedural Forest**: Poisson-disk sampling creates natural tree placement
- **Ray-Circle Trees**: Smooth cylindrical tree trunks using mathematical ray intersection
- **40×40 Unit World**: Large explorable forest with varied tree density
- **Realistic Collision**: Circle-circle collision with wall sliding around trees

### 🎨 **Atmospheric Effects**
- **Dappled Lighting**: Dynamic light filtering through canopy gaps
- **Distance Fog**: Objects fade naturally at far distances
- **Wind Effects**: Multi-layer canopy movement with organic patterns
- **Falling Leaves**: Subtle particle system with realistic physics

### 🎯 **Advanced Rendering**
- **High Resolution**: 160×60 ASCII character grid for detailed visuals
- **Dual Raycasting**: Wall DDA + tree ray-circle intersection
- **Forest Floor**: Procedural leaf litter with hash-based textures
- **Canopy Skybox**: Pseudo-parallax overhead foliage with wind

### 🎮 **Enhanced Experience**
- **Smooth Movement**: WASD controls with 2.5 units/second normalized speed
- **Look Around**: Arrow keys with ±20° pitch range
- **Rich Objects**: 15+ forest items (logs, rocks, mushrooms, flowers)
- **Performance**: Adaptive resolution scaling maintains 30+ FPS

## Controls

- **WASD**: Move through the forest
- **Arrow Keys**: Look around (up/down/left/right)
- **Esc**: Pause/Resume
- **?**: Toggle help screen
- **F1**: Toggle debug information

## Technical Details

### **Rendering Engine**
- **Resolution**: 160×60 ASCII characters (9,600 total pixels)
- **Field of View**: 66 degrees with fisheye correction
- **Tree Rendering**: Ray-circle intersection math for smooth trunks
- **Spatial Hash**: O(k) collision detection with 2.0 unit cells
- **ASCII Palette**: `██▓▓▒▒░░:.` for enhanced depth shading

### **Forest Generation**
- **Algorithm**: Poisson-disk sampling with 1.8 unit minimum spacing
- **Tree Variety**: Oak and pine types with 0.4-0.6 unit trunk radius
- **Object Placement**: Natural distribution of forest elements
- **Collision System**: Circle-circle with ≤0.05 unit penetration tolerance

### **Atmospheric Systems**
- **Dappled Light**: Hash-based light patches synchronized with canopy
- **Wind Simulation**: Sinusoidal movement with multiple noise layers
- **Particle Effects**: Sparse falling leaves with drift physics
- **Distance Fog**: Gradual fade beyond 12 units for depth

## Performance

- **Target**: 30+ FPS median, 24+ FPS p95
- **Adaptive Scaling**: Auto-reduces to 120×40 if performance drops
- **Memory Usage**: <50MB total with efficient spatial hashing
- **Optimization**: Single-pass rendering with dirty region updates

## Browser Compatibility

Optimized for modern desktop browsers:
- **Chrome/Chromium**: Full performance
- **Firefox**: Full performance  
- **Safari**: Full performance
- **Edge**: Full performance

Mobile browsers supported but desktop recommended for best experience.

## Implementation

### **Architecture**
- **Pure Vanilla JS**: No frameworks or external dependencies
- **Single HTML File**: Self-contained with embedded CSS/JS
- **Modular Design**: Clean separation of rendering, physics, and world systems
- **Performance First**: Spatial hashing, object pooling, and adaptive quality

### **Key Algorithms**
- **Raycasting**: DDA for walls + ray-circle intersection for trees
- **Collision**: Swept circle-circle with tangent sliding
- **Generation**: Poisson-disk sampling for natural tree placement
- **Lighting**: Hash-based procedural textures with wind synchronization

## Development

The forest environment demonstrates advanced ASCII rendering techniques:
- Mathematical ray-geometry intersection
- Procedural content generation
- Real-time atmospheric effects
- Performance-optimized spatial data structures

---

*An exploration of procedural 3D environments rendered entirely in ASCII characters*