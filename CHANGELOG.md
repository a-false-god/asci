# Changelog

## v2.0.0 - ASCII 3D Forest (2024)

### 🌲 Major Features
- **Complete Environment Overhaul**: Transformed from indoor room to immersive forest
- **Procedural Forest Generation**: Poisson-disk sampling creates natural tree placement
- **Advanced Tree Rendering**: Ray-circle intersection for smooth cylindrical trunks
- **40×40 Unit World**: Large explorable forest environment

### 🎨 Atmospheric Systems
- **Dappled Lighting**: Dynamic light filtering through moving canopy
- **Distance Fog**: Natural fade for objects beyond 12 units
- **Wind Effects**: Multi-layer canopy movement with organic patterns
- **Falling Leaves**: Subtle particle system with realistic drift physics

### 🔧 Technical Improvements
- **Higher Resolution**: Upgraded from 120×40 to 160×60 characters
- **Dual Raycasting**: Wall DDA + tree ray-circle intersection
- **Spatial Hashing**: O(k) collision detection for performance
- **Enhanced Physics**: Circle-circle collision with wall sliding

### 🎯 Rendering Enhancements
- **Forest Floor**: Procedural leaf litter with hash-based textures
- **Canopy Skybox**: Pseudo-parallax overhead foliage
- **Rich Objects**: 15+ forest items (logs, rocks, mushrooms, flowers)
- **Improved Palette**: Enhanced ASCII characters for better depth

### ⚡ Performance
- **Adaptive Quality**: Auto-scales resolution to maintain 30+ FPS
- **Optimized Algorithms**: Spatial data structures and efficient rendering
- **Memory Efficient**: <50MB usage with object pooling
- **Browser Optimized**: Smooth performance across modern browsers

---

## v1.0.0 - ASCII 3D Room (Original)

### Features
- Basic room environment with walls and doorways
- DDA raycasting for wall rendering
- Simple collision detection
- 120×40 resolution
- Basic sprite system for objects

### Technical
- Vanilla JavaScript implementation
- Single HTML file deployment
- Grid-based collision system
- Basic ASCII palette mapping