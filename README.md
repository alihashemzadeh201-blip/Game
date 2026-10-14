# 🎮 Letta Project — Browser Games & Simulations

A collection of **standalone, single-file** browser games and physics simulations.
No build step, no installation — **just open the HTML file in a modern browser** (Chrome / Edge recommended).

> ⚠️ Requires an internet connection: 3D/physics engines load from CDN
> ([Three.js](https://threejs.org/) via import map, [Matter.js](https://brm.io/matter-js/) via jsdelivr).

---

## ✈️ `flight-simulator.html` — Flight Simulator 3D

A full 3D flight sim with procedural terrain, snow-capped mountains, and an arcade-but-real flight model.

**Features**
- Procedural canvas textures — grass terrain, asphalt runway with markings, sky, fuselage
- Ridged mountain ranges up to ~700 m with altitude tinting (grass → rock → snow caps)
- Real takeoff: engine spool-up, prop-torque pull, *Rotate!* callout at 75 kt, retractable gear
- Real landing: ground-effect cushion, flare physics, landing-quality rating (butter / firm)
- Approach warnings: **STALL** / **SINK RATE** / **GEAR!**
- 10 glowing fly-through rings + 6 hot-air balloons to pop
- HUD with speed / altitude / vertical speed / throttle / gear + attitude indicator
- Procedural WebAudio engine, wind, and chime sounds — no audio files
- Bloom post-processing, sun + clouds, chase & cockpit cameras

**Controls**

| Key | Action |
|---|---|
| `W` / `S` | Throttle up / down |
| `↑` `↓` `←` `→` | Stick — **pull `↓` back to climb** (real yoke style) |
| `A` / `D` | Rudder / nosewheel steering |
| `G` | Landing gear up / down |
| `Space` | Wheel brake |
| `C` | Chase ↔ cockpit camera |
| `R` | Reset flight |

---

## 🌇 `Flight Simulator 3D ✈️ Golden Hour.html`

The **golden-hour edition** of the flight sim — a warm, low-sun variant with a
physical sky shader, golden atmospheric haze, and sunset lighting. Same controls, different mood.

---

## 🎾 `tennis.html` — Tennis 3D

A fast 3D tennis game with bloom-lit stadium vibes, shadows, and smooth rally physics.

**Controls:** Mouse or Arrow Keys / WASD to move & swing · `R` restart · first to the target score wins

---

## 🚗 `vehicle-sandbox.html` — Vehicle Sandbox (2D Physics)

A *Bad Piggies*-style vehicle-building sandbox powered by Matter.js.
Snap parts together, add pin / motor / piston joints, then press play and watch your creation roll (or explode).

**Features**
- One-click jointing — click an overlap of two parts to instantly pin/motor them (auto wheel-center snapping)
- Motors with configurable key bindings, pistons, springs
- Keyboard shortcuts `1–8` for tools, `Space` = Play/Stop
- Built-in pin icons, dashed joint previews, and a test harness (`sandbox_test.js`, 20 checks)

---

## 🧮 `calculator.html` — Calculator

A clean, responsive web calculator with full keyboard support.

---

## 🚀 How to run

1. Clone the repo:
   ```bash
   git clone https://github.com/alihashemzadeh201-blip/Game.git
   ```
2. Double-click any `.html` file — it opens in your browser and runs immediately.

## 🛠️ Tech

- [Three.js 0.160](https://threejs.org/) + UnrealBloom (flight sim, tennis)
- [Matter.js 0.19](https://brm.io/matter-js/) (vehicle sandbox)
- Procedurally generated textures & audio — zero asset files
