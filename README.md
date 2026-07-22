<p align="center">
  <img src="assets/logo-navy.png" width="160" alt="Naval Architecture Engineering Suite Logo">
</p>

# Naval Architecture Engineering Suite v2

> **Under active development.** Based on user feedback from v1.0.
> Built on OpenCASCADE Technology (OCCT) — the same geometry kernel as FreeCAD.

---

## What's coming

- **Faired hull surface** — real NURBS geometry via OpenCASCADE, not parametric approximation
- **Compartment modelling** — tanks, holds, voids as 3D solids inside the hull (colour coded)
- **Proper Lines Plan** — Body Plan, Sheer Plan, Half-Breadth sliced from the real OCCT surface
- **Propeller & shaft design** — B-series (Wageningen) open water curves, blade geometry, shaft arrangement
- **Deep stability** — real loading conditions, tank sounding tables, free surface per compartment
- **Project save / load** — .nasp project file format, recent projects on startup
- **Vector PDF export** — true vector charts and drawings, Excel calculation summary

---

## Project structure

```
C:\Temp\NavalArchitectureSuite_v2
│
├── Core\
│   ├── HullSurface.cs        ← OCCT NURBS hull surface
│   ├── Compartment.cs        ← OCCT solid compartments
│   ├── PropellerGeometry.cs  ← OCCT blade surfaces
│   └── OffsetTable.cs        ← Offset table import / export
│
├── Hydrostatics\             ← From OCCT volume integration
├── Stability\                ← From real compartments (Vol 29, 30)
├── DamageStability\          ← From flooding simulation (Vol 30)
├── Resistance\               ← Holtrop-Mennen + real hull form
├── Propulsion\               ← New — B-series propeller + shaft
├── LinesPlan\                ← Sliced from OCCT hull surface
│
├── Views\                    ← WPF + HelixToolkit
├── ViewModels\               ← MVVM architecture
└── Services\                 ← PDF, Excel export
```

---

## Technology stack

| Component | Technology |
|---|---|
| Language | C# / .NET 8 |
| UI Framework | WPF |
| 3D Viewport | HelixToolkit.Wpf |
| Geometry Kernel | OpenCASCADE Technology (OCCT) via Macad.Kernel |
| Charts | OxyPlot |
| PDF Export | SimplePdfDocument (custom, dependency-free) |

---

## Scientific foundation

Based on the **Naval Architecture Teaching Toolkit** — 34 volumes, 3,000+ live formulas.
All volumes are free and open educational resources.

| Volume | Title |
|---|---|
| Vol 1 | Fundamental Calculations of Naval Architecture |
| Vol 2 | Ocean Hydrodynamics & Ship Motions |
| Vol 3 | Propeller, Machinery & Marine Materials |
| Vol 4 | Structural Design & Scantlings |
| Vol 5 | Ship Manoeuvring & Control |
| Vol 6 | Submarine Engineering |
| Vol 7 | Fluid Mechanics for Naval Architects and Marine Engineers |
| Vol 8 | Damage Stability |
| Vol 9 | Introduction to Finite Element Methods for Naval Architects |
| Vol 10 | Hovercraft Engineering |
| Vol 11 | Classification Societies and Marine Regulations |
| Vol 12 | Advanced Resistance and Powering — Holtrop-Mennen 1984 |
| Vol 13 | Seakeeping and Operability |
| Vol 14 | Offshore Structures and Drilling Platforms |
| Vol 15 | Marine Corrosion and Corrosion Protection |
| Vol 16 | Marine Vibration and Noise |
| Vol 17 | Bow Design |
| Vol 18 | Gas and Steam Turbines |
| Vol 19 | Marine Diesel Engines |
| Vol 20 | Marine Auxiliary Systems |
| Vol 21 | Welding Engineering |
| Vol 22 | Shipbuilding Welding Practice |
| Vol 23 | Yacht Design |
| Vol 24 | Advanced Yacht Design |
| Vol 25 | Tonnage and Freeboard |
| Vol 26 | Damage Stability and Subdivision |
| Vol 27 | Ship Manoeuvring and Rudder Design |
| Vol 28 | LNG Cargo Systems |
| Vol 29 | Stability of Special Vessels |
| Vol 30 | Intact and Damage Stability in Depth |
| Vol 31 | Ship Manoeuvring and Hydrodynamics |
| Vol 32 | Ship Production and Outfitting |
| Vol 33 | Underwater Noise and Signatures |
| Vol 34 | Ice Class and Polar Operations |

---

## Current stable release

The current working version is v1.0 — fully functional, 14 modules, 3,358 live formulas, free installer.

⬇️ **[Download Naval Architecture Engineering Suite v1.0](https://github.com/alperalacam/NavalArchitectureSuite/releases/tag/v1.0)**

---

## Roadmap

| Phase | Scope | Status |
|---|---|---|
| 1 | OCCT proof of concept — NURBS hull in HelixToolkit | Planned |
| 2 | Hull surface engine — slicing, offset table, Lines Plan | Planned |
| 3 | Compartment modelling — solids, colours, volumes | Planned |
| 4 | Deep hydrostatics and stability from real geometry | Planned |
| 5 | Stability deep — Vol 30 formulas + compartments | Planned |
| 6 | Propeller and shaft design — B-series | Planned |
| 7 | PDF / Export — vector PDF, Excel summary | Planned |
| 8 | Release | Planned |

---

## Author

**Alper Alacam** — Naval Architect & Marine Engineer, Türkiye

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Alper_Alacam-blue)](https://www.linkedin.com/in/alper-alacam-b70b9566)
[![v1.0](https://img.shields.io/badge/Current_Release-v1.0-gold)](https://github.com/alperalacam/NavalArchitectureSuite/releases/tag/v1.0)

---

*Free to use. Free to share. Dedicated to engineers who believe knowledge should be accessible to everyone.*

© 2026 Alper Alacam — Türkiye
