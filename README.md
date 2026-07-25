<!-- ================================================================ -->
<!--  README.md  —  Mechanical Design Repository                      -->
<!--  Replace all [PLACEHOLDER] text and image paths before pushing.  -->
<!-- ================================================================ -->

<h1 align="center">[Device / Assembly Name]</h1>
<p align="center">
  <em>[One-line tagline — e.g. "30:1 Cycloidal Gearbox for the DEIMOS Mars Rover"]</em>
</p>

<p align="center">
  <img alt="status" src="https://img.shields.io/badge/status-active-brightgreen">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-blue">
  <img alt="cad" src="https://img.shields.io/badge/CAD-SolidWorks-orange">
</p>

---

## 📖 Overview

This repository contains the complete mechanical design package for **[Device Name]**, developed by **[Team / Org Name]**. It includes native CAD source files, manufacturing-ready drawings, 3D-printable/exportable mesh files, and full assembly documentation.

**Use case:** [1–2 sentences on what this device does and where it's used — e.g. "This gearbox reduces motor output speed by 30:1 to drive the rover's wheel hubs, providing high torque density in a compact housing suitable for the rocker-bogie suspension."]

### 📁 Repository Structure

| Folder | Contents | Format(s) |
|---|---|---|
| `CAD/` | Native, editable part & assembly files | `.SLDPRT`, `.SLDASM`, `.step` |
| `Drawings/` | Manufacturing / engineering drawings with GD&T, dimensions, tolerances | `.pdf`, `.SLDDRW` |
| `STL/` | Exported meshes for 3D printing, simulation, or viewing | `.stl` |
| `Renders/` | Rendered images used for documentation/marketing | `.png`, `.jpg` |
| `BOM/` | Bill of materials, part sourcing sheets | `.xlsx`, `.csv` |
| `docs/` | Supporting documentation, images used in this README | — |

> 💡 Tip: Start with `CAD/` if you plan to modify the design, `Drawings/` if you're sending parts out for manufacturing, and `STL/` if you just need to print or view geometry quickly.

---

## 🖼️ Design Preview

<table>
  <tr>
    <td width="50%">
      <img src="docs/images/render_front.png" alt="Front rendered view" width="100%">
      <p align="center"><b>Front Isometric Render</b><br>[Short description — e.g. "Assembled gearbox showing the twin-disc cycloidal stage and output flange."]</p>
    </td>
    <td width="50%">
      <img src="docs/images/render_exploded.png" alt="Exploded rendered view" width="100%">
      <p align="center"><b>Exploded View Render</b><br>[Short description — e.g. "Exploded assembly highlighting bearing placement, ring pins, and disc stack order."]</p>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <img src="docs/images/drawing_2d.png" alt="2D engineering drawing" width="100%">
      <p align="center"><b>2D Engineering Drawing</b><br>[Short description — e.g. "Full manufacturing drawing of the [part name] with critical dimensions, tolerances, and section views."]</p>
    </td>
  </tr>
</table>

---

## 🧱 Material Information

| Part | Material | Grade / Spec | Notes |
|---|---|---|---|
| [Housing] | [Aluminium] | [6061-T6] | Anodized for corrosion resistance |
| [Cycloidal Disc] | [Steel] | [EN8 / SS304] | Hardened surface preferred for pin contact |
| [Ring Pins] | [Stainless Steel] | [SS304, 6mm dia] | Ground finish for low friction |
| [Bearings] | [Chrome Steel] | [6902 series] | Sealed / shielded as specified |
| [Fasteners] | [Stainless Steel] | [A2-70] | — |
| [Output Shaft] | [Steel] | [EN24 / 4340] | — |

> Replace with your actual part list. Include hardness, surface finish, and any heat-treatment requirements where relevant.

---

## 🏭 Manufacturing Details

| Part | Process | Machine / Method | Tolerance | Notes |
|---|---|---|---|---|
| [Housing] | CNC Milling | 3-axis mill | ±0.05 mm | Requires 2 setups (front/back face) |
| [Cycloidal Disc] | Laser / Wire-EDM cutting | Wire-EDM | ±0.02 mm | Tight tolerance on lobe profile |
| [Ring Pins] | Turning | Lathe | ±0.02 mm | Ground OD for press-fit |
| [Output Flange] | CNC Milling + Drilling | 3-axis mill | ±0.05 mm | Deburr all edges before assembly |
| [Custom Bracket] | Sheet metal cutting + bending | Laser cutter + brake press | ±0.1 mm | DXF provided in `Drawings/` |

**General notes:**
- All drawings in `Drawings/` include full GD&T callouts — always manufacture from these, not raw CAD geometry.
- STL files in `STL/` are for visualization/printing only and are **not dimensionally toleranced** for CNC/EDM work.

---

## 🔧 Assembly Information

1. [Step 1 — e.g. "Press bearings into the housing bore using an arbor press; support the housing on the outer race only."]
2. [Step 2 — e.g. "Insert the eccentric shaft through the bearings."]
3. [Step 3 — e.g. "Mount the twin cycloidal discs with a 180° phase offset onto the eccentric bushings."]
4. [Step 4 — e.g. "Install ring pins into the housing, ensuring even spacing per the drawing."]
5. [Step 5 — e.g. "Fit the output flange and secure with fasteners per the specified torque sequence."]
6. [Step 6 — e.g. "Verify free rotation by hand before final closure of the housing."]

Refer to the exploded render above and the assembly drawing in `Drawings/` for exact part orientation and fastener callouts.

---

## ⚠️ Cautions — Manufacturing & Assembly

- **Tolerances:** Cycloidal disc lobe profiles are tolerance-critical — verify machined parts against the drawing before assembly; even small deviations can cause binding.
- **Bearing press-fits:** Never press bearings using the inner race when installing onto a shaft, or the outer race when installing into a housing — this can damage the balls/races.
- **Handling ground/hardened parts:** Handle hardened discs and ground pins carefully to avoid surface nicks, which can cause premature wear or noise.
- **Cleanliness:** Ensure all parts are cleaned and deburred before assembly — trapped swarf/debris is a common cause of gearbox failure.
- **Fastener torque:** Follow specified torque values; over-torquing housing fasteners can warp thin-walled sections.
- **Phase alignment:** For twin-disc cycloidal designs, confirm the 180° phase offset is correct before final fastening — incorrect phasing causes vibration and uneven load sharing.
- **Orientation:** Double-check asymmetric parts (e.g. eccentric shafts, off-center flanges) against the drawing — incorrect orientation is not always visually obvious.

---

## 📄 License

[Specify license, e.g. MIT — see `LICENSE` file for details.]

## 🙌 Credits

Developed by **[Team Name]**, [Institution/Organization].
