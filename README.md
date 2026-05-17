# ⚡ LevelUp — Personal Self-Improvement Tracker

LevelUp is a highly interactive, beautifully animated, zero-dependency, and zero-database web application designed for tracking personal growth. Built entirely in a single HTML file, it allows you to log daily achievements, maintain streaks, and visually track your progress through dynamically changing color "Laps."

Your data is natively saved to your local machine using the modern File System Access API—ensuring ultimate privacy, ownership, and effortless GitHub backups.

---

## ✨ Core Features

*   **⚡ Level Progression System**: Every meaningful task you complete (DSA problem, run, reading, etc.) increases your level by 1. Every 10 levels constitutes a "Lap."
*   **🔥 Daily Streak Tracker**: Log at least one achievement daily to keep your streak fire burning. Missing a day resets the fire, encouraging consistency.
*   **⏳ Exact Age Clock**: A real-time life clock displaying your precise age in Years, Months, and Days, calculated down to the day.
*   **📖 Achievement Journal**: Log your tasks with a specific Heading, Description, and Summary/Reflection. Empty fields flash red to ensure you don't skip the details!
*   **⏱️ Expandable & Searchable Timeline**: A beautifully animated, reverse-chronological timeline strip. Easily search past achievements by Task Number, Keywords, or using a built-in Calendar Date Picker.
*   **🖐️ Draggable UI**: The "LAP" label badge is floating and draggable—place it anywhere on your screen. Its position is automatically saved to your data file.
*   **🎉 Dual-Celebration Animations**: Enjoy a satisfying visual burst of confetti when you level up, and a massive, glowing full-screen sequence when you complete a 10-level Lap.

---

## 💾 Zero-Database Storage System

This app does not rely on external servers or cloud databases. 
1. **Auto-Save to File**: On your first visit, click the prompt at the bottom to link a local `data.json` file. 
2. **Seamless Writes**: Every time you level up, the app writes your data *directly* to that JSON file on your hard drive. 
3. **Smart Fallback**: The app uses IndexedDB to remember your file handle across sessions. If you are on an unsupported browser, it safely falls back to standard `localStorage`.

### How to Backup via GitHub
Because your data lives directly in `data.json`, backing up is as simple as committing and pushing `index.html` and `data.json` to a private GitHub repository. 

---

## 🎨 Aesthetics & UI Design

LevelUp is designed with a sleek, dark-mode, cyberpunk-meets-minimalism aesthetic. 

### Visual Elements
*   **Canvas Background**: 6 glowing color blobs slowly drift and shift continuously behind the main interface, creating a breathing, dynamic environment.
*   **Glassmorphism & Glows**: Subtle blur backdrops, neon drop-shadows, and glowing accent borders give the interface depth.
*   **Typography**: 
    *   `Bebas Neue` for big, bold, impactful numbers and headings.
    *   `Space Mono` for technical readouts, timeline dates, and labels.
    *   `Inter` for clean, readable descriptions and input fields.
*   **Micro-interactions**: Ripple effects on button clicks, bouncy number animations, and smooth CSS cubic-bezier transitions.

### 🌈 The "Lap" Color Palette System
To keep the journey visually fresh, the app completely shifts its color scheme every time you complete 10 levels (1 Lap). The circular progress ring, the horizontal XP bar, and the Lap Badge transition smoothly into new gradients.

There are 10 unique Lap palettes that loop continuously:

| Lap | Levels | Gradient Palette Colors | Hex Codes |
| :--- | :--- | :--- | :--- |
| **Lap 1** | 0 – 9 | Deep Violet to Bright Cyan | `#7c3aed` → `#06b6d4` |
| **Lap 2** | 10 – 19 | Neon Pink to Bright Orange | `#ec4899` → `#f97316` |
| **Lap 3** | 20 – 29 | Emerald Green to Bright Cyan | `#10b981` → `#06b6d4` |
| **Lap 4** | 30 – 39 | Warm Amber to Crimson Red | `#f59e0b` → `#ef4444` |
| **Lap 5** | 40 – 49 | Soft Purple to Emerald Green | `#8b5cf6` → `#10b981` |
| **Lap 6** | 50 – 59 | Bright Cyan to Neon Pink | `#06b6d4` → `#ec4899` |
| **Lap 7** | 60 – 69 | Bright Orange to Soft Purple | `#f97316` → `#8b5cf6` |
| **Lap 8** | 70 – 79 | Crimson Red to Warm Amber | `#ef4444` → `#f59e0b` |
| **Lap 9** | 80 – 89 | Emerald Green to Warm Amber | `#10b981` → `#f59e0b` |
| **Lap 10** | 90 – 99 | Fuchsia to Sky Blue | `#e879f9` → `#38bdf8` |

---

## 🚀 How to Run
1. Create a folder on your computer.
2. Place `index.html` and an empty file named `data.json` inside it.
3. Open `index.html` in any modern web browser (Chrome, Edge, Brave recommended for native File System Access).
4. Click the prompt at the bottom to link your `data.json` file.
5. Hit **⚡ LEVEL UP** and start grinding!