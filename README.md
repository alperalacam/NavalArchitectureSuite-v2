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

Based on the Naval Architecture Teaching Toolkit — 31 volumes, 3,358+ live formulas:

- **Vol 29** — Stability of Special Vessels
- **Vol 30** — Intact and Damage Stability in Depth
- **Vol 31** — Ship Manoeuvring and Hydrodynamics
- **Vol 32** — Ship Production and Outfitting *(in progress)*
- **Vol 33** — Underwater Noise and Signatures *(in progress)*
- **Vol 34** — Ice Class and Polar Operations *(in progress)*

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
| 5 | Propeller and shaft design — B-series | Planned |
| 6 | Project save/load, vector PDF, full release | Planned |

---

## Author

**Alper Alacam Naval Architecture — Concept Design Studio**
Türkiye

[![LinkedIn](https://img.shields.io/badge/LinkedIn-alperalacam-blue)](https://www.linkedin.com/in/alperalacam)
[![v1.0](https://img.shields.io/badge/Current_Release-v1.0-gold)](https://github.com/alperalacam/NavalArchitectureSuite/releases/tag/v1.0)

---

*Free to use. Free to share. Dedicated to engineers who believe knowledge should be accessible to everyone.*

© 2026 Alper Alacam Naval Architecture — Türkiye
