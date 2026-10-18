# Bangladesh 3D Interactive Map & Atlas (বাংলাদেশ ৩ডি মানচিত্র)

A standalone, interactive 3D WebGL map of Bangladesh featuring all 64 districts, 8 divisions, rivers, topography, administrative facts, and BCS geography study tools.

Inspired by and compatible with the Prottoy BCS Map interactive application.

![Bangladesh 3D Map Preview](https://raw.githubusercontent.com/placeholder/preview.png)

---

## 🌟 Key Features

- **Interactive 3D WebGL Canvas**: Smooth rotate, tilt, pan, and zoom across all 64 districts with 3D elevation and extruded division polygons.
- **8 Administrative Divisions (৮টি বিভাগ)**:
  - Dhaka (ঢাকা - ১৩টি জেলা)
  - Chattogram (চট্টগ্রাম - ১১টি জেলা)
  - Rajshahi (রাজশাহী - ৮টি জেলা)
  - Khulna (খুলনা - ১০টি জেলা)
  - Barishal (বরিশাল - ৬টি জেলা)
  - Sylhet (সিলেট - ৪টি জেলা)
  - Rangpur (রংপুর - ৮টি জেলা)
  - Mymensingh (ময়মনসিংহ - ৪টি জেলা)
- **Division Separation Mode (ম্যাপ দিয়ে আলাদা করুন)**: Highlight and separate division boundaries in 3D.
- **Search & Auto-Fly**: Real-time search by district name (বাংলা ও English), upazila, river, or landmarks with fly-to zoom animations.
- **Detailed District Fact Sheets**: Slide-out panel for any clicked district with area (বর্গকিমি), population, upazila list, historical places, geography, and BCS study points.
- **Surrounding Geography**: Neighboring regions labeled (Meghalaya, Assam, Tripura, Mizoram, West Bengal, Myanmar, Bay of Bengal).
- **Bilingual Interface**: Seamless 1-click toggle between Bengali (বাংলা) and English.
- **Zero Runtime Dependencies**: Completely self-contained HTML/WebGL bundle. Works standalone or via modern bundlers (Vite).

---

## 🚀 Quick Start

### Option 1: Standalone (No Node.js Required)
Simply open `index.html` directly in any modern web browser (Google Chrome, Microsoft Edge, Safari, Firefox).

### Option 2: Run with Vite Dev Server
```bash
# 1. Install dependencies
npm install

# 2. Start local development server
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Option 3: Production Build
```bash
npm run build
npm run preview
```
Production assets are generated in `dist/`.

---

## 🧭 URL Parameters & Deep Linking

You can deep-link into specific views or districts using query parameters or hash:

| Parameter | Description | Examples |
|-----------|-------------|----------|
| `v` | Map view mode (`division`, `district`, `rivers`, etc.) | `?v=division` |
| `d` | Focus on specific district (index / name) | `?d=dhaka`, `?d=chattogram` |
| `f` | Fullscreen / focus mode (`1` for true) | `?f=1` |

Example:
```
http://localhost:3000/?v=division
```

---

## 🌐 Deployment

This project can be deployed to any static host with zero configuration:
- **GitHub Pages**: Push to repository and enable GitHub Pages on `main` branch or `/dist` folder.
- **Vercel**: Run `vercel` or link your Git repository.
- **Netlify**: Drag and drop the root folder or `dist/`.
- **Cloudflare Pages**: Connect repo with build command `npm run build` and output directory `dist`.

---

## 📄 License

MIT License. Educational and study use.
