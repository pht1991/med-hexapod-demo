# HexaFrame 3D · Hexapod External Fixator Digital Showcase

**Live demo: https://pht1991.github.io/med-hexapod-demo/**

[简体中文](README.zh-CN.md)

A Web-based 3D interactive demo of a hexapod external fixator (Stewart platform / Taylor-frame-type structure), built with Three.js — zero build step, single-file deployment.

> For interactive visualization only — not a medical device and not a clinical calculator.

## Features

- **Real-time 6-strut inverse kinematics** — deformity parameters (varus/valgus, flexion/extension, rotation + 3D translation) drive frame deformation and bone reduction in real time
- **Adjustment prescription output** — per-strut correction Δ (S1–S6) and estimated correction period at 1 mm/day
- **Sample bone models** — full-length femur and tibia+fibula, selectable in-app, auto-aligned and split into proximal/distal segments at the fracture plane
- **STL import** — upload or drag-and-drop any `.stl` bone model; automatic long-axis alignment, ring-fit scaling, and fracture-plane segmentation
- **Parametric frame specs** — ring diameter Ø140/160/180 mm, ring spacing 250/300/350 mm, rebuilt live
- **Bilingual UI** — English / 简体中文, one-click switch
- **Random case generator** and one-click correction animation

## Customize This Engine

Built for medical device manufacturers:

- Website 3D product showcase (replaces static images)
- Interactive trade-show kiosk / large touchscreen
- Portable sales demo (runs on an iPad)
- Medical education & training

Contact via the in-app "Customize" dialog, or GitHub: [pht1991](https://github.com/pht1991)

## Run

Pure static single page — any static server works:

```bash
python3 -m http.server 8080
# or just visit the live demo above
```

## License / Credits

- Repository code: MIT
- Sample bone models (`models/femur-full.stl`, `models/tibia.stl`): segmented from CT data of a full human leg, published on [NIH 3D](https://3d.nih.gov/) — [3DPX-000168 (femur)](https://3d.nih.gov/entries/3dpx-000168) and [3DPX-000169 (tibia & fibula)](https://3d.nih.gov/entries/3dpx-000169), **CC0 1.0 (public domain)**
- This demo is for interactive visualization only and does not constitute a medical device or clinical basis
