# DistroGuess 🐧🎯

> **A Wordle/Loldle-style deduction game for Linux enthusiasts, built with pure Material Design 3 and 100% Vibe Coding.**

[![Author: vroderoot](https://img.shields.io/badge/Author-vroderoot-emerald?style=flat-square&logo=github)](https://github.com/vroderoot)
[![Engine: Gemini Argon](https://img.shields.io/badge/Engine-Gemini%20Argon-blue?style=flat-square&logo=google)](https://deepmind.google)
[![100% Vibe Code](https://img.shields.io/badge/Code-100%25%20Vibe%20Coded-purple?style=flat-square&logo=visualstudiocode)](https://github.com/vroderoot)
[![License: MIT](https://img.shields.io/badge/License-MIT-amber?style=flat-square)](LICENSE)

---

## ⚡ The "100% Vibe Code" Experiment

This entire project was conceived, structured, and crafted through **100% Vibe Coding** using Google's **Gemini Argon** model. 

### Why Vibe Coding?
The author (**vroderoot**) wanted to dive into the emerging **Vibe Coding** niche to explore the boundaries of natural language software engineering:
- **No manual boilerplate or CSS tweaking:** Architecture, UI layout tokens, game math, and reactive DOM handling were directed purely through natural dialogue and intent.
- **Procedural SVG generation:** Rather than sourcing static copyrighted image assets, the model was guided to procedurally draw vector emblems using geometric shapes and distro color codes.
- **Zero build step requirement:** The entire application lives inside a single, high-performance static HTML file that runs anywhere out of the box without Node.js, Webpack, or external bundlers.

---
---
> While checking the old name for existing projects, I found https://github.com/fedes1to/distrodle. I highly recommend checking it out.
>
---

## 🎮 Game Modes

### 1. 📅 Daily Challenge (`Задание дня`)
- Every player across the globe gets the exact same secret distribution every calendar day.
- Deterministically calculated via a custom **Mulberry32 PRNG** algorithm mapped to the current UTC date.
- Progress, guesses, and solved state persist in `localStorage`.
- Includes a live countdown timer to the next daily drop.

### 2. ♾️ Endless Mode (`Бесконечный режим`)
- Play as many rounds as you want back-to-back.
- Instant round restarts and a surrender option if you get stuck.

---

## 📊 Guess Comparison System

Each guess evaluates **8 key technical specs** against the mystery distribution:

| Spec | Match Criteria | Color Indicator |
| :--- | :--- | :--- |
| **Based On** | Exact match / Common upstream ancestor | 🟩 Exact / 🟨 Partial / 🟥 Wrong |
| **Init System** | `systemd`, `OpenRC`, `runit`, `SysVinit`, etc. | 🟩 Exact / 🟨 Partial / 🟥 Wrong |
| **Package Manager** | `pacman`, `apt`, `dnf`, `zypper`, `nix`, etc. | 🟩 Exact / 🟨 Partial / 🟥 Wrong |
| **Default Desktop (DE)** | `GNOME`, `KDE Plasma`, `Xfce`, `COSMIC`, etc. | 🟩 Exact / 🟨 Partial / 🟥 Wrong |
| **Release Model** | `Rolling`, `Fixed (Point)`, or `Hybrid` | 🟩 Exact / 🟨 Partial / 🟥 Wrong |
| **Architecture** | `x86_64`, `ARM64`, `i686` support | 🟩 Exact / 🟨 Partial / 🟥 Wrong |
| **Release Year** | Numeric year comparison with `↑` / `↓` hints | 🟩 Match / 🟨 Within ±3 yrs / 🟥 >3 yrs |

---

## 🎨 UI & Design Principles

- **Material Design 3 (MD3):** Strict tonal palette tokens (dark/light themes), pill-shaped segmented controls, elevated cards, and smooth flip animations.
- **Mobile-First Responsive Layout:**
  - **Desktop (`≥ 1024px`):** Full 8-column side-by-side comparison matrix.
  - **Mobile / Tablet (`< 1024px`):** Native card view with a 2-column parameter grid — **no horizontal scroll needed**.
  - **Swipeable Bottom Sheet:** Quick drag handles, quick-filter chips (`Debian`, `Arch`, `RPM`, `Independent`), and full-screen expand mode.
- **Bilingual Support:** 1-click instant runtime switching between **Russian** and **English** with full dictionary translations.

---

## ⚖️ Legal & Trademark Protection (100% Safe)

This project has been deliberately designed to be **safe from trademark and copyright disputes**:

1. **Procedural Geometry (Zero Trademarked Assets):**
   No proprietary logos (Canonical's circle of friends, Red Hat's shadowman, Debian's swirl, etc.) are included or hosted. All icons are purely algorithmic geometric approximations drawn with inline SVG polygons, circles, and gradients.
2. **Nominative Fair Use:**
   Distribution names, package managers, and release years are factual data used strictly to identify subjects in an educational trivia context.
3. **No Affiliation Disclaimer:**
   The application displays a non-affiliation disclaimer stating that it is an independent, non-commercial fan project not endorsed by or affiliated with The Linux Foundation, Canonical, Red Hat, SPI, or other trademark owners.

---

## 🚀 Quick Start & Deployment

### Run Locally:
No installation, npm, or build step required. Just clone and open `index.html`:
```bash
git clone https://github.com/vroderoot/distrodle.git
cd distrodle
# Open in any browser:
open index.html   # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

### Deploy to GitHub Pages:
1. Push `index.html` to your repository.
2. Go to **Settings** → **Pages**.
3. Under **Build and deployment**, select `main` (or `master`) branch `/root` folder and hit **Save**.
4. Your game is live in seconds!

---

## 👤 Author & Socials

Created with passion by **vroderoot**:

- **TikTok:** [@vroderoot](https://www.tiktok.com/@vroderoot)
- **YouTube:** [@vroderoot](https://youtube.com/@vroderoot)

---

## 📄 License

This project is open-source and released under the [MIT License](LICENSE).
