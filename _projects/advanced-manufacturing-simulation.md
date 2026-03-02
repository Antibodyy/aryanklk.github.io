---
title: "Modeling and Simulation of Advanced Manufacturing Processes"
collection: projects
type: "Graduate Course"
permalink: /projects/advanced-manufacturing-simulation
venue: "UC Berkeley"
location: "Berkeley, CA"
order: 3
---

Developed computational models and optimization algorithms for advanced manufacturing processes including robotic 3D printing, laser heating, and multi-physics simulations.

## 1. Modeling Robotic Arm-based 3D Printing

This module focused on the physics-based simulation of an Additive Manufacturing (AM) system. The model accounts for the multi-link kinematics of the robotic arm, the electrodynamic forces acting on the material droplets, and the fluid dynamics governing deposition.

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 2%; margin: 20px 0; width: 100%;">
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/robotic_arm_printer.png' | relative_url }}" alt="Robotic Arm AM Diagram" style="width: 100%; height: 300px; object-fit: contain; background: #fff; border-radius: 8px; border: 1px solid #eee;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Schematic of the modeled Arm-based AM System</em></p>
    </div>
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/robotic_3D_printer.gif' | relative_url }}" alt="Robotic 3D Printer Simulation" style="width: 100%; height: 300px; object-fit: contain; background: #000; border-radius: 8px;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Deposition Simulation & Pattern Formation</em></p>
    </div>
</div>

### Key Technical Implementations:
* Modeled robotic 3D printing systems by developing forward kinematics for multi-link robot arms, computing droplet dynamics under electromagnetic forces and drag.
* Implemented Forward Euler time-stepping to simulate material deposition with electrodynamic field control for precise pattern formation.
* Analyzed multi-physics phenomena combining electromagnetic field interactions and fluid dynamics (Reynolds number-dependent drag) to enable predictive modeling.

---