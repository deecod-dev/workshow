﻿# DRDO Terrain Pathfinding Hack

A hybrid Python→Java solution to accelerate DTED2-based military pathfinding by 95%+, prototyped in hours and productionized in days.

---

## 📂 Repository Structure

```
.
├── docs/
│   ├── contours.png         # Drawn contours avoiding no-go regions
│   └── paths.png            # Final optimal paths
├── src/
│   ├── python_prototype/
│   │   └── prototype.py
│   └── java_backend/
│       ├── DTED2Reader.java
│       └── PathfinderEngine.java
├── tests/
│   └── regression_tests.py
└── README.md
```

---

## 🚀 Overview

During a DRDO research internship, our team faced 25 min+ delays running BFS/A\* on large DTED2 elevation maps. I devised a creative hack:

1. **Python Prototype**

   * Custom DTED2 reader using NumPy & SciPy
   * Fast Marching Method (FMM) tuned to slopes and no-go zones
   * Quick visualization checks

2. **Java Production**

   * Multi-threaded path engine
   * JavaFX integration into the JAYANT backend

---

## 📈 Visuals

### Contour Map (No-Go Regions)

Shows the elevation contours and areas to avoid:

![Contours](contours.png)

### Computed Paths

Overlay of optimal routes computed by the hack:

![Paths](paths.png)

---

## 🗝 Access

The core codebase for this project is proprietary and restricted under DRDO policies. It is not publicly available in this repository. Documentation, diagrams, and high-level descriptions are provided here for overview purposes only.

## 👤 Author

Dev Utkarsh Pal
Research Intern @ DRDO & IIIT‑Delhi
📧 [dev22150@iiitd.ac.in](mailto:dev22150@iiitd.ac.in)

---

## 📄 License

This project is licensed under the DRDO internal NDA. 🔒
