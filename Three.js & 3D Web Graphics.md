---
title: Three.js & 3D Web Graphics Architecture
type: technology-hub
category: creative-engineering-3d
tags:
  - tech/threejs
  - tech/webgl
  - tech/r3f
  - tech/rapier
  - frontend/creative-dev
projects:
  - "[[Janver Manlapaz — 3D Interactive Developer Portfolio — Complete Project Architecture & Knowledge Base|Janver Manlapaz Portfolio]]"
---

# Three.js & 3D Web Graphics Architecture

> [!INFO] **Technology Overview**
> Real-time 3D graphics and physics simulations in the browser using **WebGL**, **Three.js**, **React Three Fiber (@react-three/fiber)**, and the **Rapier** WebAssembly physics engine.

---

## Core 3D Architecture Stack

```mermaid
graph TD
    ReactApp[React 18 & Vite Frontend] --> Canvas3D[R3F Canvas Container]
    
    subgraph WebGL Rendering Pipeline
        Canvas3D --> Scene[Three.js Scene Graph]
        Scene --> Camera[Perspective Camera & Controls]
        Scene --> Lights[Ambient & Directional Lighting]
        Scene --> Character[3D Character Model & Rigging]
        Scene --> PostProcessing[Post-processing & Bloom Filters]
    end
    
    subgraph Physics Engine
        Scene --> Physics[Rapier / Cannon Physics World]
        Physics --> Colliders[Rigid Body Colliders]
        Physics --> Gravity[Gravity & Impulse Vectors]
    end
    
    subgraph Game Engines
        ReactApp --> ChessEngine[Stockfish.js & Chess.js AI Arena]
    end
```

---

## Key Capabilities Implemented
1. **React Three Fiber (R3F)**: Declarative component-driven Three.js scene graphs integrated directly with React state and lifecycle hooks.
2. **WASM Physics (Rapier / Cannon)**: Real-time collision detection, bone ragdolls, and tactile particle physics.
3. **Smooth Motion Choreography**: Lenis virtual smooth scroll combined with GSAP scroll-triggered timeline animations.
4. **Post-Processing**: Depth of field, bloom, and chromatic aberration optimized for 60+ FPS on consumer GPUs.

---

## Projects Implementing 3D & WebGL
- [[Janver Manlapaz — 3D Interactive Developer Portfolio — Complete Project Architecture & Knowledge Base|Janver Manlapaz: 3D Interactive Developer Portfolio]]

---

## Related Hubs
- [[Tailwind CSS]]
- [[Home|Projects Dashboard]]
