```markdown
<div align="center">

# 🧠 Memory Match

### *Flip, Find & Match the Pairs!*

A vibrant, child-friendly memory card matching game built with pure HTML, CSS & JavaScript — no frameworks, no dependencies, just one file.

[![Play Now](https://img.shields.io/badge/▶_Play_Now-Live_Demo-FFD54F?style=for-the-badge&logoColor=black&labelColor=FFD54F&color=FFA000)](https://your-username.github.io/memory-match/)
[![License](https://img.shields.io/badge/License-MIT-4FC3F7?style=for-the-badge)](LICENSE)
[![Single File](https://img.shields.io/badge/Single_File-HTML-FF80AB?style=for-the-badge)](index.html)

<br>

<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white"/>
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>

</div>

---

## 🎮 Gameplay Preview

<table>
  <tr>
    <td align="center"><b>Welcome Screen</b></td>
    <td align="center"><b>Game in Progress</b></td>
    <td align="center"><b>Victory Screen</b></td>
  </tr>
  <tr>
    <td><img src="https://via.placeholder.com/300x500/FFF8F0/FF80AB?text=Welcome+Screen" width="300"/></td>
    <td><img src="https://via.placeholder.com/300x500/FFF8F0/4FC3F7?text=Gameplay" width="300"/></td>
    <td><img src="https://via.placeholder.com/300x500/FFF8F0/FFD54F?text=Victory!+🎉" width="300"/></td>
  </tr>
</table>

> 📸 *Replace placeholder images with actual screenshots of your game*

---

## ✨ Key Features

### 🃏 Core Gameplay
| Feature | Description |
|---------|-------------|
| 🔄 **3D Card Flip** | Smooth CSS 3D perspective flip animation with backface visibility |
| 🎯 **Match Detection** | Real-time pair matching with visual + audio feedback |
| 🔒 **Anti-Cheat** | Double-click protection & input lock during card comparison |
| 📊 **Live Stats** | Move counter, timer & pair tracker updating in real-time |

### 🎚️ Difficulty Levels

| Level | Grid | Pairs | Best For |
|-------|------|-------|----------|
| 🌱 **Simple** | 4 × 3 | 6 pairs | Young kids & beginners |
| ⚡ **Medium** | 4 × 4 | 8 pairs | Casual players |
| 🔥 **Difficult** | 6 × 4 | 12 pairs | Memory masters |

### 🎨 Visual & Audio Effects

- 🌈 **Gradient-shifting title** with animated color cycling
- 🎪 **Floating background shapes** — soft decorative blobs in constant motion
- ✨ **Star burst particles** explode from matched cards
- 🎊 **Confetti rain** (80 pieces, 3 shapes) on victory
- 🏆 **Star rating** — earn 1–3 stars based on move efficiency
- 🔊 **Synthesized sound effects** via Web Audio API — no audio files needed
  - *Flip click* · *Match chime* · *Mismatch tone* · *Victory arpeggio*
- 💫 **Shimmer effect** on the Start button with sliding highlight
- 🃏 **6 alternating card-back gradients** for visual variety

---

## 🚀 Quick Start

### Option 1: Just Open It
```bash
# Clone the repo
git clone https://github.com/your-username/memory-match.git

# Open in browser — that's it!
open memory-match/index.html
```

### Option 2: Live Server (VS Code)
```bash
# Install Live Server extension, then:
# Right-click index.html → Open with Live Server
```

### Option 3: GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Source: `Deploy from a branch` → `main` → `/ (root)`
4. Your game is live at `https://your-username.github.io/memory-match/`

> ✅ **Zero dependencies.** No `npm install`, no build step, no server required.

---

## 🏗️ Technical Architecture

### Single-File Structure

```
index.html
├── <style>          → All CSS (variables, animations, responsive)
├── <body>           → Three screen views (Welcome / Game / Win)
│   ├── #welcomeScreen
│   ├── #gameScreen
│   └── #winScreen
└── <script>         → Complete game engine
    ├── Audio Engine      → Web Audio API sound synthesis
    ├── Screen Manager    → View transitions & state
    ├── Game Logic        → Cards, matching, scoring
    ├── Effects Engine    → Particles, confetti, toasts
    └── Timer & Stats     → Real-time tracking
```

### Design Decisions

| Decision | Why |
|----------|-----|
| **Single HTML file** | Zero setup, instant play, easy sharing |
| **Web Audio API** | No external audio files, instant loading |
| **CSS 3D transforms** | GPU-accelerated flips, no JS animation overhead |
| **CSS custom properties** | Centralized theming, easy color customization |
| **No framework** | Maximum portability, no build pipeline |
| **Tailwind via CDN** | Utility classes for rapid layout, no local install |

---

## 🎨 Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| 🟦 Sky Blue | `#4FC3F7` | Card backs, accents, stat values |
| 🟨 Bright Yellow | `#FFD54F` | Start button, gold effects, highlights |
| 🩷 Candy Pink | `#FF80AB` | Card backs, toasts, result stats |
| 🟩 Mint Green | `#A5D6A7` | Card backs, easy difficulty accent |
| 💗 Neon Pink | `#FF6EC7` | Play-again button, particles, glow |
| 🩵 Neon Blue | `#00E5FF` | Confetti, particles, special effects |
| 🥇 Gold | `#FFD700` | Matched card borders, stars, shimmer |
| 🍦 Warm White | `#FFF8F0` | Background, card fronts |

---

## 🔧 Customization Guide

### Change Card Symbols
Edit the `SYMBOLS` array in the `<script>` section:
```javascript
const SYMBOLS = [
    '🌟', '🦋', '🌈', '🎈', '🍭', '🎪',
    '🐱', '🐶', '🌺', '🍎', '🎵', '🦄',
    // Add or replace any emoji you like!
];
```

### Change Colors
Edit CSS custom properties in `:root`:
```css
:root {
    --sky-blue: #4FC3F7;
    --bright-yellow: #FFD54F;
    --candy-pink: #FF80AB;
    --mint-green: #A5D6A7;
    /* Change these to retheme the entire game */
}
```

### Add a New Difficulty
Add an entry to `DIFFICULTY_CONFIG`:
```javascript
const DIFFICULTY_CONFIG = {
    easy:   { cols: 4, rows: 3, pairs: 6 },
    medium: { cols: 4, rows: 4, pairs: 8 },
    hard:   { cols: 6, rows: 4, pairs: 12 },
    // Try: extreme: { cols: 6, rows: 6, pairs: 18 }
};
```

---

## ♿ Accessibility

- ♿ **Keyboard navigation** — Tab through cards, Enter/Space to flip
- 🏷️ **Dynamic ARIA labels** — Cards announce state to screen readers
- 🎬 **`prefers-reduced-motion`** — All animations disabled for users who prefer it
- 👆 **Touch-friendly** — Large tap targets, responsive card sizing
- 📱 **Mobile-first** — Grid reflows on small screens (6-col → 4-col)

---

## 🌐 Browser Support

| Browser | Status |
|---------|--------|
| Chrome 80+ | ✅ Full support |
| Firefox 75+ | ✅ Full support |
| Safari 14+ | ✅ Full support |
| Edge 80+ | ✅ Full support |
| Mobile Safari | ✅ Full support |
| Mobile Chrome | ✅ Full support |

> Requires `transform-style: preserve-3d` and Web Audio API support.

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute.

```text
MIT License

Copyright (c) 2026 Memory Match

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including, without limitation, the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

<div align="center">

**Made with ❤️ and pure HTML/CSS/JS**

⭐ If you like this project, give it a star on GitHub!

[⬆ Back to Top](#-memory-match)
