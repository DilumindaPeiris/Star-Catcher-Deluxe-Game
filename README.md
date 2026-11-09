# 🌟 Star Catcher — Deluxe Edition

[![License: MIT](https://img.shields.io/badge/License-MIT-amber.svg)](LICENSE)
[![HTML5 Canvas](https://img.shields.io/badge/HTML5-Canvas%202D-orange.svg)](#technical-architecture)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio-Procedural%20Synth-cyan.svg)](#procedural-audio-engine)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-v3.4-38bdf8.svg)](#)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-emerald.svg)](#)

An ultra-responsive, arcade-style celestial tap game built with pure vanilla JavaScript, HTML5 Canvas, procedural Web Audio API synthesis, and Tailwind CSS. Catch falling stars, trigger game-changing cosmic combos, dodge dark void hazards, and set records across three unique game modes!

---

## 🎮 Play Live

Play **Star Catcher Deluxe** instantly on GitHub Pages:
👉 **[Play Star Catcher Deluxe Live](https://dilumindapeiris.github.io/Star-Catcher-Deluxe-Game/)**

---

## ✨ Features

- 🌌 **Retina-Ready 2D Canvas Engine**: Fluid 60 FPS graphics with HiDPI display scaling, dynamic cosmic grid, and procedural twinkling starfields.
- ⚡ **Dynamic Combo & Frenzy System**: Chain rapid star catches within 2.2 seconds to ramp multipliers up to **5x**, igniting a chaotic **Star Frenzy** mode.
- 🎵 **Procedural Web Audio Synth**: 100% code-synthesized sound effects (pentatonic chords, crystal bells, bass drops, and ambient space drone)—no heavy MP3s or audio files needed.
- 💥 **Juicy Visual Feedback**: Screen shake, shockwave rings, floating score popups, and gravity-driven stardust particle bursts.
- 🏆 **3 Engaging Game Modes**:
  - **⏱️ Time Attack**: 30-second high-intensity rush; earn extra time by collecting Chrono and Gold stars.
  - **❤️ Classic (3 Lives)**: Survival test with 3 hearts; avoid misses and dodge hazardous Space Bombs.
  - **✨ Zen Chill**: Relaxing, infinite star-catching session with zero timers, zero lives, and zero bombs.
- 📊 **Lifetime Pilot Statistics**: LocalStorage-backed tracking for total stars caught, maximum combo streaks, games played, accuracy percentages, and mode high scores.
- 📱 **Mobile & Desktop Friendly**: Touch-optimized hit detection with cursor stardust trails and keyboard shortcuts.

---

## 🌠 Celestial Star Codex

| Star Archetype | Point Value | Visual Appearance | Special Ability |
|---|:---:|---|---|
| **Gold Star** | `100 pts` | Radiant Golden 5-Point Star | Base celestial star. Adds `+0.5s` in Time Attack. |
| **Supernova** | `250 pts` | Deep Violet 4-Point Star | **Board Clear**: Detonates a cosmic shockwave that automatically collects all active stars! |
| **Frost Star** | `150 pts` | Crystalline Cyan 6-Point Star | **Time Freeze**: Slows all star movement to 25% speed for 4 seconds with a frost border. |
| **Chrono Star** | `150 pts` | Emerald 5-Point Star with Clock | **Time Warp**: Instantly grants `+4.0s` bonus time in Time Attack mode. |
| **Rainbow Comet** | `500 pts` | Rapid Shifting 7-Point Comet | **Star Frenzy**: Doubles all point yields (`2x`) and spawns extra stars for 5 seconds. |
| **Dark Void Bomb** | `-200 pts` | Pulsing Crimson 8-Point Hazard | **Hazard Penalty**: Deducts 200 points, resets combo, shakes screen, and deducts 1 heart in Classic mode! |

---

## 🕹️ Controls & Hotkeys

| Action | Mouse / Touch | Keyboard Shortcut |
|---|---|:---:|
| **Catch Star** | Left-Click / Tap on Star | — |
| **Pause / Resume** | Click Pause button (`⏸`) | <kbd>Space</kbd> |
| **Quick Restart** | Click Restart button | <kbd>R</kbd> |
| **Close Modals** | Click Close button | <kbd>Esc</kbd> |
| **Toggle SFX** | Click SFX icon (`🔊`) | — |
| **Toggle Ambient Music** | Click Music icon (`🎵`) | — |

---

## 🛠️ Technical Architecture

- **Zero External Dependencies**: Operates entirely in a standalone browser context without npm builds, node servers, or asset packs.
- **Procedural Audio Engine**:
  - Web Audio API `AudioContext` generating sine, triangle, and sawtooth waves.
  - Harmonic pentatonic chord frequencies: `[523.25Hz, 587.33Hz, 659.25Hz, 783.99Hz, 880.00Hz, 1046.50Hz]`.
  - Ambient algorithmic space drone generating gentle pentatonic arpeggios on a 1600ms interval.
- **Physics & Particle Pipeline**:
  - Independent velocity integration (`x += vx * timeScale`, `y += vy * timeScale`).
  - Elastic boundary reflection with radius cushioning.
  - Stardust particles featuring alpha decay and gravitational curvature (`vy += 0.05`).

---

## 🚀 Local Development

1. **Clone the repository**:
   ```bash
   git clone https://github.com/DilumindaPeiris/Star-Catcher-Deluxe-Game.git
   cd Star-Catcher-Deluxe-Game
   ```

2. **Open the game**:
   - Double-click `index.html` to launch in any modern web browser.
   - Or serve with any static web server (e.g. `npx serve` or VS Code Live Server).

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.
