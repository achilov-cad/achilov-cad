# Automotive Body Panel Reverse Engineering & Stamping Die Design (Matrix + Punch)

Engineering project focused on reconstructing smooth Class-B CAD surfaces from a raw 3D scan and designing a two-piece stamping die set (**Matrix + Punch**) for forming **1.0 mm** sheet metal.

## 🎯 Project Objectives
1. Convert a noisy polygonal 3D scan (`.stl`) of a double-curved automotive body panel with a fuel door recess into a clean, watertight parametric CAD model (`.step`).
2. Design a matched **Matrix and Punch** tooling set suitable for 3D printing / CNC machining with a precise **1.0 mm** clearance gap for sheet metal stamping.

## 🛠 Tools & Workflow
* **Software:** Autodesk Fusion 360 (Surface & Solid Modeling)
* **Base Surface Reconstruction:** Extracted reference cross-sections (`Mesh Section Sketch`), traced profiles using uniform Degree-3 `Control Point Splines`, and generated a smooth base surface via `Surface Loft`.
* **Recess Modeling:** Trimmed the fuel door opening (`Trim`), extruded draft walls along the stamping axis (`Extrude Direction + Taper Angle`), patched the bottom, stitched surfaces (`Stitch`), and applied transition radii (`Fillet`).
* **Tooling & Clearance:** Generated a `1.0 mm` offset surface (`Surface Offset`) to account for sheet metal thickness and split solid stock blocks (`Split Body`) into the final Matrix and Punch components.

*(Note: Production `.step` files are withheld to respect commercial client confidentiality).*

