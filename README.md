# 🏰 Wizard's Chess 3D — Gothic Cathedral

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen?style=for-the-badge&logo=github)](https://isbandurahuman-r.github.io/3D-CHESS/)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![Chess.js](https://img.shields.io/badge/Chess.js-0.10.3-blue?style=for-the-badge)](https://github.com/jhlywa/chess.js)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-v3-38bdf8?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

> An immersive, Harry Potter–inspired **Wizard's Chess** game rendered in full 3D inside a vaulted Gothic Cathedral. Watch pieces violently strike down enemies and shatter them into exploding stone debris, accompanied by procedural acoustic audio!

---

## ✨ Features

- 💥 **Violent Shatter Combat**: Captures trigger cinematic strike animations where the captured piece shatters into high-speed physics shards and debris.
- 🏰 **Atmospheric Gothic Cathedral**: Built with procedural Three.js architecture featuring soaring ribbed vaults, arched colonnades, torchlight lanterns, and stained-glass lighting.
- 🧠 **Dual Game Modes**:
  - **Wizard AI**: Battle an arcane AI opponent with heuristic minimax evaluation.
  - **2-Player Local**: Pass-and-play against a friend on the same screen.
- ♟️ **Full FIDE Chess Validation**: Powered by `chess.js` — handles legal moves, checks, checkmates, stalemates, castling, en passant, and pawn ascension (promotion modal).
- 🔮 **Arcane Move Guidance**:
  - Legal move tile highlights and hover targeting runes.
  - "Arcane Hint" button to suggest optimal strategic moves.
  - "Test Shatter" button to instantly preview destruction animations.
- 🔊 **Procedural Web Audio Synthesizer**: 100% synthesized in real time via the Web Audio API — resonant stone slides, heavy warhammer impact thuds, crystalline shard clatters, and ethereal check chimes (no external audio files required!).
- 💎 **Material Design 3 Glassmorphism HUD**:
  - Live turn indicators with check warnings.
  - Captured pieces graveyard and dynamic material advantage counter.
  - Interactive "Chronicle of Moves" history log.
  - Camera preset switcher (White POV, Black POV, Overhead Tactical, and Free Orbit).
- ⚡ **Zero-Build Architecture**: Everything is bundled into a single standalone static web page with CDN assets. No `npm install`, webpack, or build scripts needed!

---

## 🎮 Controls

| Action | Control |
| :--- | :--- |
| **Select Piece / Move** | **Left Click** on piece or target square |
| **Orbit Camera** | **Click & Drag** anywhere on the background |
| **Zoom In / Out** | **Mouse Scroll Wheel** or pinch gesture |
| **Cycle Camera Angles** | Click the **Cam Preset** button on the top bar |
| **Arcane Hint** | Click **Hint** to illuminate the best move |
| **Undo Move** | Click **Undo** to take back your last move |
| **Toggle Audio** | Click **SFX On / Off** |

---

## 🚀 Quick Start (Play Locally)

Since this game is built as a pure web app, you can run it immediately without any installation:

### Option 1: Direct File Open
Simply double-click [`index.html`](index.html) or `wizard_s_chess_gothic_cathedral_3d.html` to open it in Chrome, Edge, Firefox, or Safari.

### Option 2: Local HTTP Server (Recommended)
Running through a local web server ensures optimal WebGL performance and audio context initialization:

- **Using Python 3**:
  ```bash
  python -m http.server 8000
  ```
  Then visit `http://localhost:8000` in your browser.

- **Using Node.js (`npx serve`)**:
  ```bash
  npx serve .
  ```

- **Using VS Code Live Server**:
  Right-click `index.html` and choose **"Open with Live Server"**.

---

## 🌐 Deploy to GitHub Pages (Play Online for Free)

You can host this game on the web so anyone can play it in their browser for free using GitHub Pages:

1. Push this repository to GitHub (see the [GitHub Push Guide](#-how-to-push-to-github) below).
2. Go to your repository on **GitHub.com**.
3. Click on **Settings** (gear icon) > **Pages** (in the left sidebar).
4. Under **Build and deployment** > **Branch**:
   - Select `main` (or `master`)
   - Select `/ (root)` folder
   - Click **Save**.
5. Wait 1–2 minutes, and GitHub will provide your live URL:
   `https://isbandurahuman-r.github.io/3D-CHESS/`

---

## 🛠️ How to Push to GitHub

### 1. Initialize Git and Commit
Open your terminal in this folder and run:

```bash
git init
git add .
git commit -m "Initial commit: Wizard's Chess 3D in Gothic Cathedral"
```

### 2. Create a Repository on GitHub
1. Log in to [GitHub](https://github.com/).
2. Click the **`+`** icon in the top right corner and select **New repository**.
3. Name your repository `3D-CHESS`.
4. Set visibility to **Public** (required for free GitHub Pages).
5. **Do NOT** check "Add a README" or ".gitignore" (we already created them!).
6. Click **Create repository**.

### 3. Link Remote and Push
```bash
git branch -M main
git remote add origin https://github.com/ISBANDURAHUMAN-R/3D-CHESS.git
git push -u origin main
```

---

## 📂 Project Structure

```text
├── index.html                           # Main entry point (compatible with GitHub Pages)
├── wizard_s_chess_gothic_cathedral_3d.html  # Original standalone single-file distribution
├── .gitignore                           # Git ignore rules for system and editor cache files
└── README.md                            # Documentation and deployment guide
```

---

## 🧰 Built With

- [Three.js](https://threejs.org/) (r128) — 3D WebGL rendering, lighting, materials, and particle simulations
- [Chess.js](https://github.com/jhlywa/chess.js) — FIDE chess rule validation and legal move calculation
- [Tailwind CSS](https://tailwindcss.com/) — Clean, responsive glassmorphism UI styling
- [Google Fonts](https://fonts.google.com/) — *Cinzel* (Gothic header typography) & *Inter* (UI readability)
- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) — Real-time synthesized sound effects

---

## 📜 License

This project is open-source and released under the [MIT License](LICENSE). Feel free to customize, enhance, and enjoy!
