# Doppleit 3D Pro

**A modular 3D creative engine for the browser.**  
Real-time object manipulation, animation, physics, and plugin extensibility — all in one file.

---

## ✨ Features

- 🎮 **Transform Controls**  
  Select, move, rotate, and scale 3D objects in a live scene

- 🧱 **Primitive & Asset Library**  
  Add cubes, spheres, cones, torus, planes, and drag in GLTF/GLB models

- 🧠 **Timeline + Keyframes**  
  Animate position, rotation, and scale with keyframe interpolation

- 💡 **Inspector Panel**  
  Live object editing: transform, visibility, shadows, color, and more

- 🔁 **Undo / Redo**  
  Full state history with deep scene memory restoration

- 🧲 **Physics Engine**  
  Toggle Cannon.js physics with dynamic body assignment per object

- 🎞️ **Post-Processing**  
  Bloom rendering via EffectComposer + UnrealBloomPass

- 📊 **Performance Overlay**  
  Live FPS, object count, and memory usage display

- 🧩 **Plugin System**  
  Register tools and listeners using `DoppleitAPI`

---

## 📦 Tech Stack

- [Three.js](https://threejs.org/)  
- [Cannon-ES](https://github.com/pmndrs/cannon-es)  
- [GLTFLoader](https://threejs.org/docs/#examples/en/loaders/GLTFLoader)  
- [EffectComposer](https://threejs.org/docs/#examples/en/postprocessing/EffectComposer)  
- Built in **pure JS/HTML/CSS** — no frameworks required

---

## 🔌 DoppleitAPI (Plugin Example)

```js
DoppleitAPI.register("MyPlugin", {
  init(api) {
    console.log("Doppleit plugin initialized!");
  },
  onEvent(event, data) {
    if (event === "object.created") {
      console.log("New object:", data);
    }
  }
});
```

---

## 🚀 Getting Started

1. Clone or download the repo  
2. Open `index.html` in any modern browser  
3. Start creating — no build step needed

---

## 📁 Roadmap

- DoppleitAPI plugin store (v1.1)  
- Asset tagging + thumbnails  
- SVG/PNG export system  
- Multi-user sync (WebSocket)  
- Material editor & node graph  
- Integrated version control

---

## 💬 License

MIT — built with reflection, recursion, and love.

---