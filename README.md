<img width="2240" height="1260" alt="VorCore 10 Custom CoreXY Gantry Mounts" src="https://github.com/user-attachments/assets/b5744e2e-e804-494b-b272-d1cf7a5e575c" />

# VorCore 10: Custom CoreXY Gantry Mounts

VorCore 10 is a custom-designed, open-source CoreXY kinematic mounting system. It bridges the gap between the heavy-duty front-motor layout of the SolidCore and the clean, stacked belt routing made popular by Voron designs.

Optimized and tested for a large, rigid 1000x1000x500mm build volume, this system is built entirely around wider 10mm GT2 belts to handle aggressive accelerations without stretching or skipping.

## Design Lineage & Features

- **SolidCore Inspiration:** X and Y stepper motors are front-mounted, pushing the center of gravity forward and freeing up space at the rear of the machine.
- **Voron-Style Routing:** The belts route across the front of the X-axis extrusion in a stacked configuration, ensuring clean, parallel belt paths rather than looping behind the starting belt.
- **Heavy-Duty 10mm Belts:** Dimensioned strictly for 10mm GT2 belts and matching hardware to eliminate belt stretch on high-speed setups.

## The Kinematic System & Belt Routing

The VorCore 10 system utilizes standard CoreXY kinematics for its belt routing, making it familiar and straightforward to configure. The mounting system consists of four purpose-built modules designed for easy printing, assembly, and maintenance. _(Note: The Front, Center, and Back modules are required in pairs—one set for the left gantry and one set for the right.)_

<img width="768" height="610" alt="CoreXY-Kinematics" src="https://github.com/user-attachments/assets/0c748690-ec8d-49f3-8d17-eadeaacb2292" />

1. **Front (Motor Mount):** Rigidly holds the NEMA 17 stepper motors in the front corners.
2. **Center (Extrusion Clamp):** Securely grips the X-axis extrusion and maintains perfect alignment for the front-stacked belt path.
3. **Back (Idler Mount):** Houses the rear idler pulleys to return the belts through the kinematic path.
4. **Print Head Belt Adapter:** The crucial anchoring point that cleanly terminates the 10mm stacked belts at the toolhead, ensuring perfect parallel alignment with the X-axis.

## Bill of Materials (BOM)

Below is the total hardware required to build the complete X/Y gantry system.

**Front (Motor Mounts - Left & Right Pair)**

- 12x M3x8 bolts (6 per side)
- 2x 10mm Motor Pulley (1 per side)

**Center (Extrusion Clamps - Left & Right Pair)**

- 4x M5x8 bolts (2 per side, for attaching to 20mm V-Slot Gantry Plate)
- 4x M5x25 bolts (2 per side, for the idlers)
- 4x M3x8 bolts (2 per side, for attaching to the extrusion)
- 2x 10mm GT2 Idlers with teeth (1 per side)
- 2x 10mm GT2 Idlers without teeth / smooth (1 per side)

**Back (Idler Mounts - Left & Right Pair)**

- 2x M5x40 bolts (1 per side, for the idler stack)
- 4x 10mm GT2 Idlers with teeth (2 per side)

**Print Head Belt Adapter (Single Unit)**

- 2x M5x8 bolts (for attaching to 20mm V-Slot Gantry Plate)
- _Note: The adapter includes extra bolt slots for mounting a BLTouch, or other custom toolhead accessories. Feel free to explore and modify!_

## CAD & Source Files

This project was designed entirely in Onshape. To make modifications, adjust for different extrusion profiles, or tweak hole tolerances, you can copy the public workspace directly:

- **[Link to Public Onshape Document](https://cad.onshape.com/documents/c695cb2f7fbb45d5485f2701/w/7bdce7ef937412e146022feb/e/c0170e9e5d0967ed7b441d22?renderMode=0&uiState=6a2ffd77a922eda218ee8340)**

For users who just want to print and assemble, the exported STLs and high-resolution STEP files are included in the `files` directory.

## Recommended Print Settings

To ensure the mounts have the rigidity required to handle 10mm belt tension and high accelerations, please follow these minimum printing guidelines:

- **Material:** ABS, ASA, or PC (PETG can work, but avoid PLA as it will creep under belt tension and motor heat)
- **Wall Loops / Perimeters:** 4
- **Top / Bottom Shells:** 5
- **Infill:** 40% (Grid, Gyroid, or Honeycomb)
- **Layer Height:** 0.2mm

## License

This project is fully open-source. Feel free to download, modify, remix, and share your own upgrades!

---

_VorCore 10 by ironerae_
