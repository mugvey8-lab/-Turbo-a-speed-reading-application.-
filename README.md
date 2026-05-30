<div align="center">

<img width="120" src="https://raw.githubusercontent.com/your-username/turbo/main/assets/logo.png" alt="Turbo Logo" />

# ⚡ TURBO

### *Read faster. Think deeper. Learn more.*

**A science-backed speed reading PWA powered by RSVP + ORP technology**

<br/>

[![Version](https://img.shields.io/badge/version-1.0.0-F5A623?style=flat-square)](https://github.com/your-username/turbo/releases)
[![PWA Ready](https://img.shields.io/badge/PWA-ready-5A0FC8?style=flat-square&logo=pwa&logoColor=white)](https://web.dev/progressive-web-apps/)
[![Offline](https://img.shields.io/badge/works-offline-22C55E?style=flat-square&logo=serviceworker&logoColor=white)](#pwa-installation)
[![License: MIT](https://img.shields.io/badge/license-MIT-3B82F6?style=flat-square)](LICENSE)
[![Languages](https://img.shields.io/badge/lang-EN%20%7C%20UZ-E11D48?style=flat-square)](#localization)
[![No Dependencies](https://img.shields.io/badge/dependencies-zero-64748B?style=flat-square)](#tech-stack)

<br/>

[**🚀 Live Demo**](#) &nbsp;·&nbsp; [**📖 How It Works**](#-how-it-works) &nbsp;·&nbsp; [**📲 Install App**](#-pwa-installation) &nbsp;·&nbsp; [**🤝 Contribute**](#-contributing)

<br/>

---

</div>

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Screenshots](#-screenshots)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [How to Use](#-how-to-use)
- [PWA Installation](#-pwa-installation)
- [Why Speed Reading?](#-why-speed-reading)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)

<br/>

---

## 🧠 Overview

**Turbo** is a zero-dependency, installable Progressive Web App that trains you to read **2–5× faster** using two clinically studied techniques: **RSVP** (Rapid Serial Visual Presentation) and **ORP** (Optimal Recognition Point) highlighting.

> Paste any text. Set your speed. Hit play. Your brain does the rest.

It works entirely in your browser — no accounts, no tracking, no server. Install it once and it works forever, even offline. Built for readers in **English** and **O'zbek (Uzbek)**.

<br/>

---

## ✨ Features

<table>
<tr>
<td width="50%">

### ⚡ Core Reading Engine
| | Feature | Description |
|---|---|---|
| ⚡ | **RSVP Mode** | One word at a time, center-fixed — zero eye movement |
| 🎯 | **ORP Highlight** | Accent on the brain's natural recognition anchor in each word |
| 🎚️ | **Speed Control** | Fine-tune WPM from 100 (beginner) to 1000+ (advanced) |
| ▶️ | **Playback Controls** | Play · Pause · Reset — full session control |

</td>
<td width="50%">

### 📱 App & Accessibility
| | Feature | Description |
|---|---|---|
| 🌐 | **EN / UZ i18n** | Complete UI in English and Uzbek |
| 📲 | **Installable PWA** | Home screen install on any device |
| 🔌 | **Offline First** | Fully cached — works with no internet |
| 📋 | **Text Input** | Paste or type any text to begin |

</td>
</tr>
</table>

<br/>

---

## 🔬 How It Works

### ⚡ RSVP — Rapid Serial Visual Presentation

Traditional reading has two silent speed killers:

```
👁️  Eye movement  →  physically scanning left-to-right across each line
🗣️  Subvocalization  →  your inner voice "pronouncing" every word
```

RSVP eliminates **both** by flashing one word at a time at a fixed center point on screen. Your eyes stay locked. Your brain decodes words directly — no scanning, no inner speech. The result:

```
Average reader          →   238 WPM
RSVP beginner           →   300–400 WPM
RSVP trained            →   500–700 WPM
RSVP advanced           →   1000+ WPM
```

<br/>

### 🎯 ORP — Optimal Recognition Point

Cognitive research shows the brain doesn't process a whole word at once — it fixates on a single character located **~30% from the left edge**. This is the **Optimal Recognition Point**.

Turbo highlights the ORP in each word with an accent color, aligns it to a fixed position on screen, and lets your brain lock on instantly — like a targeting reticle for your reading.

```
Word         →    ORP position    →    Turbo renders it as
─────────────────────────────────────────────────────────
"the"        →    position 1      →    t[h]e
"reading"    →    position 2      →    r[e]ading
"speed"      →    position 2      →    s[p]eed
"faster"     →    position 2      →    f[a]ster
"brain"      →    position 2      →    b[r]ain
```

> `[x]` = the highlighted ORP character (displayed in accent color in the app)

Together, RSVP + ORP compound each other's benefits: **faster delivery + faster recognition = exponential reading speed gains.**

<br/>

---

## 📸 Screenshots

> 📷 *Screenshots will be added here. Contributions welcome — see [Contributing](#-contributing).*

| Input Screen | Reading Session | Speed Controls |
|:---:|:---:|:---:|
| `screenshots/input.png` | `screenshots/reading.png` | `screenshots/speed.png` |
| Paste your text and set WPM | Words flash one-by-one with ORP | Fine-tune speed on the fly |

<br/>

---

## 🛠️ Tech Stack

```
turbo/
├── index.html          ← Single-page app shell
├── style.css           ← All styles, themes, animations
├── app.js              ← RSVP engine, ORP algorithm, UI logic
├── i18n.js             ← EN / UZ localization strings
├── sw.js               ← Service Worker (cache-first, offline)
└── manifest.json       ← PWA manifest (icons, theme, shortcuts)
```

| Layer | Technology | Notes |
|---|---|---|
| **UI** | Vanilla HTML5 + CSS3 | Zero frameworks, zero build step |
| **Logic** | JavaScript ES6+ | Modules, async/await, WeakMap |
| **Offline** | Service Worker API | Cache-first strategy |
| **Install** | Web App Manifest | Icons, shortcuts, display mode |
| **i18n** | Custom EN / UZ module | Lightweight, no external library |
| **Deploy** | Any static host | GitHub Pages, Netlify, Vercel, Cloudflare |

> **Zero dependencies. Zero build tools. Zero configuration.** Just open `index.html`.

<br/>

---

## 🚀 Getting Started

### Prerequisites

A modern browser is all you need (Chrome 80+, Firefox 75+, Safari 14+, Edge 80+).
No Node.js. No package manager. No compilation.

### Clone & Run

```bash
# 1. Clone the repo
git clone https://github.com/your-username/turbo.git
cd turbo

# 2. Serve locally (pick one)
python3 -m http.server 8080         # Python — built-in, always available
npx serve .                          # Node.js — one-liner, no install
npx http-server . -p 8080           # Alternative Node.js option

# 3. Open in browser
open http://localhost:8080
```

> ⚠️ **Note:** Service Workers only activate on `localhost` or `https://` origins.
> Opening `index.html` directly via `file://` will disable PWA and offline features.

### Deploy in 60 Seconds

```bash
# GitHub Pages
git push origin main
# → Enable Pages in repo Settings → Source: main branch

# Netlify (drag & drop)
# → Go to netlify.com → "Add new site" → drag the turbo/ folder

# Vercel
npx vercel deploy
```

<br/>

---

## 📖 How to Use

```
Step 1 ──► Choose language       Toggle EN / O'zbek in the top-right corner
Step 2 ──► Paste your text       Any article, book chapter, document, or note
Step 3 ──► Set your WPM          Start at 250–300 WPM (new) or 500+ WPM (trained)
Step 4 ──► Press ▶️  Play         Words flash at center; ORP character highlighted
Step 5 ──► Control as needed     ⏸ Pause · ▶ Resume · 🔄 Reset
Step 6 ──► Adjust on the fly     Change WPM mid-session without losing your place
```

**💡 Tips for beginners:**
- Start at `250 WPM` and increase by `50 WPM` each session
- Short sessions (5–10 min) build the habit faster than long marathons
- Read familiar content first — it's easier for the brain to adapt
- Don't try to subvocalize. Trust your eyes and the ORP guide

<br/>

---

## 📲 PWA Installation

Install Turbo directly to your device — no App Store, no Google Play.

<table>
<tr>
<td width="33%">

### 📱 iOS (Safari)

1. Open Turbo in **Safari**
2. Tap the **Share** button `⎋`
3. Scroll → **"Add to Home Screen"**
4. Tap **"Add"**

✅ Turbo icon appears on home screen

</td>
<td width="33%">

### 🤖 Android (Chrome)

1. Open Turbo in **Chrome**
2. Tap **⋮** menu (top-right)
3. Tap **"Add to Home screen"**
4. Tap **"Install"**

✅ Launches like a native app

</td>
<td width="33%">

### 🖥️ Desktop (Chrome/Edge)

1. Open Turbo in **Chrome** or **Edge**
2. Click **⊕** icon in address bar
3. Click **"Install"**

✅ Opens in its own app window

</td>
</tr>
</table>

> 🔌 Once installed, Turbo runs **100% offline**. The Service Worker caches all assets on first load. No internet required after that.

<br/>

---

## 🧬 Why Speed Reading?

The average adult reads at **238 WPM** — a speed bottlenecked not by intelligence, but by physical habits formed in childhood: eye movement and subvocalization.

**What the research says:**

| Finding | Source |
|---|---|
| Eye fixations account for ~90% of reading time | Rayner et al., 2016 |
| Subvocalization caps speed near speech rate (~150 WPM) | Carver, 1990 |
| RSVP readers reach 400–600 WPM with comprehension intact | Schotter et al., 2014 |
| ORP alignment cuts saccadic regression by ~15% | Beymer & Russell, 2005 |
| Speed gains transfer partially to traditional reading | Taylor, 1965 |

**The key insight:** your brain can process language far faster than your eyes and voice allow. RSVP and ORP don't bypass comprehension — they remove the *mechanical bottlenecks* that slow it down.

> 📚 Further reading: *"Breakthrough Rapid Reading"* – Peter Kump &nbsp;|&nbsp; *"The Speed Reading Book"* – Tony Buzan &nbsp;|&nbsp; Dr. Keith Rayner's eye movement research, UC San Diego

<br/>

---

## 🗺️ Roadmap

```
v1.0  ✅  RSVP engine · ORP highlighting · EN/UZ i18n · PWA/offline
v1.1  🔲  Dark / light theme toggle
v1.2  🔲  Progress bar + session percentage complete
v1.3  🔲  Reading history + WPM stats over time
v1.4  🔲  Chunked mode (2–3 words at a time)
v1.5  🔲  Font size and typeface customization
v2.0  🔲  Additional languages (Russian, Arabic, French)
v2.1  🔲  PDF / EPUB direct import
v2.2  🔲  Accessibility audit + screen reader support
```

Have an idea? [Open a feature request →](https://github.com/your-username/turbo/issues/new?template=feature_request.md)

<br/>

---

## 🤝 Contributing

Contributions are what make open source remarkable. All levels of experience welcome.

### Quick Start

```bash
# 1. Fork the repo on GitHub, then:
git clone https://github.com/YOUR-USERNAME/turbo.git
cd turbo

# 2. Create a feature branch
git checkout -b feat/your-feature-name

# 3. Make your changes, then commit
git add .
git commit -m "feat: add dark mode toggle"
# Use conventional commits: feat · fix · docs · style · refactor · test · chore

# 4. Push and open a Pull Request
git push origin feat/your-feature-name
```

### Good First Issues

- 🌙 Dark / light theme toggle
- 📊 WPM progress bar during session
- 🔤 Font size selector
- 🌍 Add Russian (`ru`) translations to `i18n.js`
- 📸 Add app screenshots to `/screenshots`
- ♿ Accessibility improvements (ARIA labels, keyboard nav)

### Bug Reports

Please [open an issue](https://github.com/your-username/turbo/issues/new?template=bug_report.md) with:
- Browser + OS
- Steps to reproduce
- Expected vs actual behavior
- Screenshot (if applicable)

<br/>

---

## 📄 License

```
MIT License — Copyright (c) 2025 Turbo Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

See [LICENSE](LICENSE) for full text.

<br/>

---

<div align="center">

**Built with ⚡ by [your-username](https://github.com/your-username) and [contributors](https://github.com/your-username/turbo/graphs/contributors)**

<br/>

*If Turbo helped you read faster, consider giving it a ⭐ — it helps others find the project.*

<br/>

[![Star on GitHub](https://img.shields.io/github/stars/your-username/turbo?style=social)](https://github.com/your-username/turbo)
[![Follow](https://img.shields.io/github/followers/your-username?style=social)](https://github.com/your-username)

<br/>

[⬆ Back to top](#-turbo)

</div>
