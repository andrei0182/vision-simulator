# Machine Vision Inspection Simulator

Single-file browser app (HTML + inline JS/CSS). 3D scene of an inspection bench with an In-Sight camera, lens, light and a part. It checks whether the setup works and can solve for a working one.

## Files

- `index.html` — the shipped app. Offline build: three.js r128 + OrbitControls inlined (~0.7 MB). No external requests.

Hosted via GitHub Pages (branch `main`, root).

A CDN-loading variant exists as the source form; the offline build is the same code with the libraries inlined.

## Solder joint inspection (lipituri)

- `lipituri/index.html` — 3D simulator of a laser-profiler station (fixed Cognex DS925B, linear axis + 0°/90° rotary table) inspecting flat pins soldered on a PCB: two scans, height maps, live laser profile, wetted-length and fillet-height checks, frame–PCB gap. Generic part, didactic model. Same offline build (three.js r128 inlined).
- Live (RO): https://andrei0182.github.io/vision-simulator/lipituri/
- Live (EN): https://andrei0182.github.io/vision-simulator/lipituri/en.html

## Tray loading inspection (tava)

- `tava/index.html` — 3D simulator of a tray-loading station: SCARA robot shows the underside of every part to a bottom camera (IS8905) before placing it, and a 25 MP camera (IS3925) inspects the full 6 × 10 tray in one image (result per pocket, DMC count, automatic replacement of NOK parts). Generic part, didactic model, offline build.
- Live: https://andrei0182.github.io/vision-simulator/tava/
