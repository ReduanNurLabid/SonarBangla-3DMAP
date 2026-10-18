# ADR 0001: SonarBangla3D Brand Identity, UI/UX Redesign, and Architecture Decoupling

## Status
**Accepted** (2026-10-18)

## Context
The project was seeded from an interactive 3D WebGL map of Bangladesh. In its initial state, the application inherited proprietary styling signatures, color schemes, legacy DOM class names (`.glass`, `#b-home`, `#b-view`, `#vmenu`), and specific trivia text from an existing platform.

To establish **SonarBangla3D** as an independent, legally defensible, and enterprise-grade commercial/educational application, we must eliminate any visual and code-level attribution to third parties, modernize the UI/UX architecture, and set up an extensible foundation for future interactive layers (including a Bangladesh GeoGuessr game).

## Decision Drivers
1. **Intellectual Property Safety**: Zero shared visual trademarks, DOM class signatures, or proprietary branding.
2. **Professional UI/UX Quality**: Clean, executive-level design tokens (WCAG 2.1 AA accessible, responsive typography, modern frosted glass HUD).
3. **Phased Delivery**:
   - **Phase 1 (Baseline)**: Rebranding to SonarBangla3D, complete UI/UX overhaul, theme engine, and signature scrubbing.
   - **Phase 2 (Enhancements)**: Bangladesh GeoGuessr interactive game, historical & thematic layers.
4. **Performance & Standalone Portability**: Retain 60 FPS WebGL rendering with zero external runtime dependencies.

## Considered Options
- **Option A: Shallow CSS Tweaks**: Change a few colors and logo. *(Rejected: Leaves structural DOM classes, layout, and visual fingerprints intact).*
- **Option B: Phased Clean Decoupling & Complete UI Redesign**: Completely re-skin and replace the UI layer with custom semantic components, introduce an extensible theme engine, scrub legacy IDs/classes, and re-architect data layers. *(Accepted)*

## Decision
We will execute **Option B** in structured phases:

1. **Brand Identity**:
   - Primary Name: `SonarBangla3D` (বাংলা: `সোনার বাংলা ৩ডি`).
   - Emblem: Custom vector-crafted geometric golden crest with emerald delta lines.
2. **Design Tokens & UI System**:
   - Design System: Cyber-Emerald / Deep Slate design tokens.
   - Palette: Deep Emerald (`#062319`), Electric Emerald (`#10B981`), Midnight Slate (`#0B132B`), Amber Gold (`#F59E0B`), and Clean Studio Light mode.
   - Component Architecture:
     - `sb-hud-topbar`: Floating capsule navigation with shortcut-enabled search (`Ctrl+K`).
     - `sb-dossier-panel`: Sleek, modular statistical drawer replacing the legacy left glass box.
     - `sb-controls`: Ergonomic camera orientation and zoom controls.
3. **Codebase Hygiene**:
   - Rename all IDs and CSS classes using the `sb-` namespace.
   - Decouple CSS into clean design token layers (`tokens.css`, `components.css`).
   - Remove all legacy copy and replace with verified administrative data (BBS 2022 Census).

## Consequences
- **Positive**: Complete visual and architectural differentiation; eliminates copyright/plagiarism risks; establishes clean design tokens for future features (like GeoGuessr).
- **Trade-off**: Requires careful DOM binding to ensure the underlying Three.js canvas listeners continue communicating seamlessly with the new HUD and Dossier controls.
