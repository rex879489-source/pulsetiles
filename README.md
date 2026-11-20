# PulseTiles 🎵🎹

A mobile-first, installable **Progressive Web App (PWA)** music-tile rhythm game. Load **any local audio file** from your phone or computer—PulseTiles analyzes the audio in your browser, extracts beats and tonal brightness into 4 beat-synced lanes, and loops each completed track into faster levels!

---

## ✨ Features

- **Play Any Local Audio File**: Supports `.mp3`, `.wav`, `.m4a`, `.ogg`, and more—decoded locally in the browser with zero server uploads.
- **Built-in Beat & Tone Extraction**: Uses the Web Audio API + an in-browser FFT Spectral Flux analyzer to detect musical onsets and map low-to-high tonal content across the 4 lanes.
- **Endless Speed-Up Levels**: Completing a song finishes the level and restarts the same beat-synced track faster (`1.00x` → `1.15x` → `1.30x` → `1.45x`…).
- **Difficulty Modes**: Switch between **Chill**, **Normal**, and **Intense** tile density.
- **Built-in Synth Demo**: Test gameplay immediately with a procedural synth track without selecting a file.
- **Mobile & Fullscreen Ready**: Multi-touch lane tapping, `100dvh` portrait layout, 60/120fps HTML5 Canvas rendering, and fullscreen toggle.
- **Installable PWA + Offline Support**: Installable to your phone's home screen with offline caching via Service Worker.

---

## 📁 Project Structure

```text
├── index.html      # Complete game UI, audio analyzer, canvas renderer & SW registration
├── manifest.json   # PWA web app manifest (fullscreen display, orientation, icon)
├── sw.js           # Service worker for offline caching
├── icon.svg        # App icon
└── README.md       # Documentation