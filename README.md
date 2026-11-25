# Machine Vision Inspection Simulator

Single-file browser app (HTML + inline JS/CSS). 3D scene of an inspection bench with an In-Sight camera, lens, light and a part. It checks whether the setup works and can solve for a working one.

## Files

- `index.html` — the shipped app. Offline build: three.js r128 + OrbitControls inlined (~0.7 MB). No external requests.

Hosted via GitHub Pages (branch `main`, root).

A CDN-loading variant exists as the source form; the offline build is the same code with the libraries inlined.

## Solder joint inspection (lipituri)

- `lipituri/index.html` — 3D simulator of a laser-profiler station (fixed Cognex DS925B, linear axis + 0°/90° rotary table) inspecting flat pins soldered on a PCB: two scans, height maps, live laser profile, wetted-length and fillet-height checks, frame–PCB gap. Generic part, didactic model. Same offline build (three.js r128 inlined).
- Live: https://andrei0182.github.io/vision-simulator/lipituri/
