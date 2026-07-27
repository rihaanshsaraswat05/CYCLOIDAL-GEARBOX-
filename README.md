<!-- ================================================================ -->
<!--  README.md  —  Mechanical Design Repository                      -->
<!--  Replace all [PLACEHOLDER] text and image paths before pushing.  -->
<!-- ================================================================ -->

<h1 align="center"> 3D PRINTED CYCLOIDAL GEARBOX </h1>
<p align="center">
  <em>["30:1 Cycloidal Gearbox for steering , actuation joints of arm link1 & 2 Mars Rover"]</em>
</p>

<p align="center">
  <img alt="status" src="https://img.shields.io/badge/status-active-brightgreen">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-blue">
  <img alt="cad" src="https://img.shields.io/badge/CAD-SolidWorks-orange">
</p>

---

## 📖 Overview

This repository contains the complete mechanical design package for **[CGB]**, developed by **[RIHAANSH SARASWAT MECH LEAD]**. It includes native CAD source files, manufacturing-ready drawings, 3D-printable/exportable mesh files, and full assembly documentation.

**THIS GEAR BOX IS A PROTOTYPE VERSION OF THE MARKET LEVEL CYCLOIDAL GEARBOX WITH 3D PRINTED CARBON FIBER INDUCED FILAMENT IT PROVIDES AN IDEAL 30:1 GEAR REDUCTION USING 2 PHASE CYCLOIDAL DISCS IWTH 31 RING PINS AND 6 DOWEL PINS THIS VERSION USES A NON BACKDRIVABLE WORM GEARED MOTOR AND A FLEXIBLE JAY COUPLING IN ORDER TO TEST AND MALFUCTION FOR ANY USE** 

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
      <img src="https://github.com/rihaanshsaraswat05/CYCLOIDAL-GEARBOX-/blob/main/photos/renderd%201.png" alt="Front rendered view" width="100%">
      <p align="center"><b>Front Isometric Render</b><br>[Short description — e.g. "Assembled gearbox showing the twin-disc cycloidal stage and output flange."]</p>
    </td>
    <td width="50%">
      <img src="https://github.com/rihaanshsaraswat05/CYCLOIDAL-GEARBOX-/blob/main/photos/rendered%202.png" alt="Exploded rendered view" width="100%">
      <p align="center"><b>Exploded View Render</b><br>[Short description — e.g. "Exploded assembly highlighting bearing placement, ring pins, and disc stack order."]</p>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <img src="https://github.com/rihaanshsaraswat05/CYCLOIDAL-GEARBOX-/blob/main/photos/drawing%20info.png" alt="2D engineering drawing" width="100%">
      <p align="center"><b>2D Engineering Drawing</b><br>[Short description — e.g. "Full manufacturing drawing of the Cycloidal gearbox with critical dimensions, tolerances, and section views."]</p>
    </td>
  </tr>
</table>

---

## Manufacturing Details

| Part | Manufacturing Process | Material | Specifications | Notes |
|------|------------------------|----------|----------------|-------|
| **Bottom Plate** | FDM 3D Printing | PLA | 0.20 mm layer height, 70–80% infill | Print with the mounting face on the build plate. Ensure bearing bores are dimensionally accurate. Avoid support material inside bearing seats. |
| **Top Plate** | FDM 3D Printing | PLA | 0.20 mm layer height, 70–80% infill | Print with the bearing seat facing upward for better dimensional accuracy. |
| **Cycloidal Disc** | FDM 3D Printing | PLA-CF / PPA-CF | 0.16–0.20 mm layer height, 80–100% infill | Print flat on the build plate. High-strength material is required due to continuous pin contact and wear. |
| **Output Shaft** | FDM 3D Printing | PPA-CF / PLA-CF | 0.16–0.20 mm layer height, 60–80% infill | Print vertically with 4–6 walls to maximize strength around the bearing seats. |
| **Eccentric Shaft** | FDM 3D Printing | PPA-CF / PLA-CF | 0.16–0.20 mm layer height, 60–80% infill | Print vertically with thick walls for maximum concentricity and strength. |
| **External Hub** | FDM 3D Printing | PLA | 0.20 mm layer height, 40–60% infill | Medium infill is sufficient. Ensure proper fit with the ring pins. |
| **Ring Pins** | CNC Turning / Precision Ground Rod | SS304 Stainless Steel | Ø6 mm Ground Rod | Maintain tight diameter tolerance and smooth surface finish for low friction. |
| **External Shaft** | CNC Turning | SS304 Stainless Steel | As per drawing | Maintain interference fit dimensions with the 10 mm shaft. |
| **10 mm Shaft** | CNC Turning | SS304 Stainless Steel | Ø10 mm | Ensure accurate bearing and coupler fit with smooth surface finish. |
| **Bearings** | Standard Purchased Component | Chrome Steel | 6902 Series | Use sealed/shielded bearings. Avoid applying assembly force through the rolling elements. |
| **Fasteners** | Standard Purchased Component | Stainless Steel | A2-70 | Use the specified tightening torque during final assembly. |
| **Coupler** | Standard Purchased Component | Aluminum | Flexible Shaft Coupler | Select bore sizes according to the motor shaft and 10 mm shaft dimensions. |
| **Thrust Washer** | Standard Purchased Component | Hardened Steel | Ø10 mm ID | Lubricate lightly with silicone spray during assembly. |

> **Manufacturing Notes**
>
> - Deburr all machined components before assembly.
> - Verify all press-fit dimensions before installing bearings and shafts.
> - Clean all bearing seats and shaft surfaces before assembly.
> - Apply silicone spray only to the shaft and thrust washer interface; avoid contaminating bearing races.
> - Check dimensional tolerances of all 3D-printed parts before assembly, especially bearing bores, shaft holes, and ring pin holes.
> - Ream printed holes if necessary to achieve the specified interference or clearance fit.
> - Inspect printed parts for warping or layer separation before use.

**General notes:**
- All drawings in `Drawings/` include full GD&T callouts — always manufacture from these, not raw CAD geometry.
- STL files in `STL/` are for visualization/printing only and are **not dimensionally toleranced** for CNC/EDM work.

---

## 🔧 Assembly Information

1. **Mount the shaft coupler** onto the motor shaft, ensuring proper alignment and securely tightening the set screws as per the specified torque.

2. **Press-fit the bearings** into the bottom plate using an arbor or hydraulic press, ensuring force is applied only to the bearing's outer race.

3. **Press-fit the ring pins** into the bottom plate and simultaneously install the external hub, ensuring all pins are fully seated and positioned according to the assembly drawing.

4. **Press-fit the external shaft** onto the 10 mm shaft, ensuring proper alignment and a secure interference fit.

5. **Press-fit the 15 mm bearing** onto the eccentric shaft by applying force only to the bearing's inner race.

6. **Insert the 10 mm shaft** into the bottom plate while installing the 10 mm thrust washer. Apply a light coating of silicone spray to the mating surfaces to facilitate assembly and reduce friction.

7. **Mount the motor** onto the bottom plate and connect it to the shaft using the pre-installed coupler. Secure the motor with the specified fasteners.

8. **Install the cycloidal discs** onto the eccentric shaft, ensuring the discs are correctly oriented and phased according to the design.

9. **Press-fit the bearings** into the output shaft and install all 8 mm dowel pins in their designated locations.

10. **Assemble the output shaft** with the cycloidal discs and install the output shaft support, ensuring smooth engagement of all output pins.

11. **Press-fit the bearings** into the top plate, applying force only to the bearing's outer race.

12. **Assemble the top plate** onto the output shaft assembly, align all mounting holes, and secure the complete gearbox using the long M4 bolts. Tighten the bolts uniformly in a crisscross sequence using a drill machine, followed by final torque tightening as specified.

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
This project is licensed under the MIT License. See the `LICENSE` file for details.

## 🙌 Credits

Developed by **RIHAANSH SARASWAT**, TEAM DEIMOS , IIT MANDI.
