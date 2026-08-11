# Overland Body — LC79 / HJ79 3D Configurator

An interactive browser-based 3D configurator created as a portfolio project for an overland camping/expedition vehicle body.

The experience presents a fully modeled camper body with an exterior view, transparent cutaway/layout view, interactive doors and storage compartments, water-tank access, interior components, chassis, ground grid, labels, camera controls, and a live part editor. The model is based on measured dimensions and reference drawings represented directly in the source.

## Highlights

- Interactive real-time 3D camper/overland body visualization
- Exterior and Cutaway + Layout viewing modes
- Multiple design-revision states with a current full-fit-out V3
- Interactive outer door and screen door controls
- Storage bench doors with independent controls
- Shower door interaction
- Water-tank doors and drawer controls
- Editable 3D parts with:
  - Fore/Aft positioning
  - Left/Right positioning
  - Up/Down positioning
  - Independent X/Y/Z scaling
  - Pitch / yaw / roll rotation
  - Individual reset and reset-all controls
- LC79 cab/chassis visibility toggle
- Layout labels and ground-grid toggles
- Optional auto-rotation
- Mouse, touch and wheel-based camera interaction
- Procedurally generated textures for corrugated panels, mesh screening, tire tread, tire sidewalls and wheel faces
- Responsive UI for smaller screens
- Portfolio contact information integrated into the interface

## Technologies Used

### Core Web Technologies

- **HTML5** — page structure, semantic controls and application container
- **CSS3** — layout, responsive styling, panels, buttons, typography, transitions, gradients and media queries
- **JavaScript (ES6+)** — application logic, UI state, 3D scene construction, interactions and animation

### 3D / Graphics

- **Three.js r128** — real-time 3D rendering and scene management
- **WebGL** — GPU-accelerated rendering through Three.js
- **Three.js MeshStandardMaterial** — physically inspired material/shading setup
- **Three.js BufferGeometry / ShapeGeometry / BoxGeometry / CylinderGeometry** — procedural model construction
- **Three.js lighting and shadows** — hemisphere, directional lighting and soft shadow mapping
- **Three.js Fog and PerspectiveCamera** — depth atmosphere and perspective presentation
- **Three.js Sprite / SpriteMaterial** — in-scene layout labels
- **Three.js CanvasTexture** — procedural texture generation and mapping

### Browser APIs

- **Canvas 2D API** — procedural texture creation and label rendering
- **DOM API** — dynamic controls, panels, dropdowns and UI state
- **Pointer Events API** — mouse/stylus camera interaction
- **Touch Events API** — touch and pinch-zoom interaction
- **Wheel Events API** — scroll-wheel zoom
- **Keyboard Events API** — shortcut controls (`1`, `2`, `E`)
- **CSS Media Queries** — responsive behavior

### Delivery

- **Three.js CDN** — Three.js is loaded directly from cdnjs
- **Static HTML deployment** — no backend, database or build system is required
- **GitHub Pages compatible** — can be deployed as a static portfolio/demo page

## Interaction Controls

| Action | Control |
|---|---|
| Orbit camera | Drag |
| Zoom | Scroll wheel / pinch |
| Pan | Shift + Drag |
| Exterior view | `1` |
| Cutaway + Layout | `2` |
| Edit Parts | `E` |
| Auto-rotate | UI toggle |

## Model / Configuration

The current V3 configuration includes the full fit-out: bunks, wet bath/shower-toilet area, storage bench, twin water tanks, spare wheel, folding seat, double entry door and cab hatch.

The source defines the primary shell dimensions as:

- Length: **3000 mm**
- Width: **2200 mm**
- Rear ramp: **700 mm**
- Wall height: **1550 mm**
- Roof height: **1950 mm**
- Roof inset/chamfer: **400 mm**

These values and the component layout are implemented directly in the HTML/JavaScript source.

## Portfolio Author

**Moiz Ahmad**

- Email: moizahmad418@gmail.com
- LinkedIn: https://www.linkedin.com/in/moizahmad418

## Notes

This is a self-contained interactive portfolio/demo implementation. It does not use a server-side application or database. Three.js is the only external JavaScript dependency and is loaded from cdnjs.

For best results, open the project in a modern desktop or mobile browser with WebGL support.
