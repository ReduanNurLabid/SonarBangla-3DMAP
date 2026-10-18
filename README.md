# SonarBangla3D (সোনার বাংলা ৩ডি)
### Interactive 3D Bangladesh Atlas & Geographic Knowledge Engine

[![GitHub Repository](https://img.shields.io/badge/GitHub-SonarBangla--3DMAP-emerald?logo=github)](https://github.com/ReduanNurLabid/SonarBangla-3DMAP.git)
[![License: MIT](https://img.shields.io/badge/License-MIT-amber.svg)](LICENSE)
[![Framework: Standalone WebGL](https://img.shields.io/badge/Engine-WebGL%20%2F%20Three.js-blue.svg)](https://threejs.org)

**SonarBangla3D** is an interactive, standalone 3D atlas and geographic exploration platform for Bangladesh. It renders the entire country in 3D perspective with 64 administrative districts, 8 divisions, river networks, topography, and real-time search.

---

## 🌟 Key Features

- **Interactive 3D WebGL Engine**: Smooth 360° orbit, camera tilt, pan, and zoom with 60 FPS performance.
- **8 Administrative Divisions (৮টি বিভাগ)**:
  - Dhaka (ঢাকা - ১৩টি জেলা)
  - Chattogram (চট্টগ্রাম - ১১টি জেলা)
  - Rajshahi (রাজশাহী - ৮টি জেলা)
  - Khulna (খুলনা - ১০টি জেলা)
  - Barishal (বরিশাল - ৬টি জেলা)
  - Sylhet (সিলেট - ৪টি জেলা)
  - Rangpur (রংপুর - ৮টি জেলা)
  - Mymensingh (ময়মনসিংহ - ৪টি জেলা)
- **3D Division Separation Mode (ম্যাপ দিয়ে আলাদা করুন)**: Dissect and elevate division islands in 3D space.
- **Keyboard-Enabled Omnibar Search**: Instant autocomplete search with `Ctrl + K` or `/` shortcut and smooth camera fly-to animations.
- **Multi-Theme Engine**:
  - 🌿 **Cyber Emerald** (Default)
  - 🌌 **Midnight Slate**
  - 👑 **Sunset Gold**
  - ☀️ **Daylight Studio**
- **Surrounding Geography**: Labeled cross-border regions (*Meghalaya, Assam, Tripura, Mizoram, West Bengal, Myanmar, Bay of Bengal*).
- **Bilingual Interface**: 1-click toggle between Bengali (বাংলা) and English.
- **Zero Runtime Dependencies**: Completely self-contained client-side bundle.

---

## 🚀 Getting Started

### Local Development
```bash
# 1. Clone the repository
git clone https://github.com/ReduanNurLabid/SonarBangla-3DMAP.git
cd SonarBangla-3DMAP

# 2. Install dev dependencies
npm install

# 3. Start development server
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Production Build
```bash
npm run build
npm run preview
```
Production assets are generated in `dist/`.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + K` or `⌘K` | Focus Search Bar |
| `/` | Quick Search |
| `Esc` | Clear Search / Close Panels |

---

## 🧭 Architecture Decision Records (ADR)

All foundational architectural decisions are documented under `/docs/adr`:
- [ADR 0001: SonarBangla3D Brand Identity, UI/UX Redesign, and Architecture Decoupling](docs/adr/0001-brand-ui-differentiation-and-engine-decoupling.md)

---

## 🗺️ Roadmap & Upcoming Upgrades

- [ ] **Bangladesh GeoGuessr Game (ম্যাপ অনুমান)**: Pin the district based on photo clues, monuments, and cultural landmarks.
- [ ] **1971 Liberation War Sectors Layer**: Interactive visualization of the 11 wartime sectors and commanders.
- [ ] **Ancient Bengal Janapadas**: Historical overlay of *Banga, Pundra, Gauda, Samatata, Harikela*.
- [ ] **National Megaprojects**: Interactive pins for Padma Bridge, Metro Rail, Karnaphuli Tunnel, and Rooppur.

---

## 📄 License

MIT License. Designed and maintained for open geographic education.
