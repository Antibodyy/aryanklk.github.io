---
title: "Metal Hydride-Based Vehicle Cooling System"
collection: projects
type: "Undergraduate Project"
permalink: /projects/metal-hydride-cooling
venue: "BITS Pilani"
location: "Pilani, India"
order: 6
---

Achieved an 18.8% reduction in auxiliary cooling power for hydrogen fuel cell vehicles through a novel metal hydride-based thermal management architecture.

## System Architecture & Integration

The cooling system is integrated directly into the US Department of Energy (DoE) FCEV reference model, replacing or augmenting traditional vapor compression cycles with a metal hydride heat pump.

<figure style="text-align: center; margin: 0 auto 30px auto; display: block; width: 100%;">
    <img src="{{ '/mhcs_ovr.png' | relative_url }}" alt="FCEV Architecture with MHCS" style="max-width: 85%; height: auto; display: inline-block; border-radius: 8px; border: 1px solid #eee;">
    <figcaption style="margin-top: 10px; color: #666;"><em>Overall hydrogen FC vehicle architecture with integrated metal hydride cooling.</em></figcaption>
</figure>

## Functional Design & Strategy

The high-level functioning plan outlines the synchronization between hydrogen flow, heat exchange, and the adsorption/desorption cycles required for continuous cooling.

<figure style="text-align: center; margin: 0 auto 30px auto; display: block; width: 100%;">
    <img src="{{ '/into_mhcs.png' | relative_url }}" alt="System Functioning Plan" style="max-width: 75%; height: auto; display: inline-block; border-radius: 8px;">
    <figcaption style="margin-top: 10px; color: #666;"><em>High-level operational workflow of the MHCS.</em></figcaption>
</figure>

---

## Modeling & Simulation

### US DoE Model Integration
To ensure industry-standard validity, the system was integrated into the **US Department of Energy's FCEV Simulink reference model**, allowing for system-level energy analysis.

<figure style="text-align: center; margin: 0 auto 30px auto; display: block; width: 100%;">
    <img src="{{ '/usdoe.png' | relative_url }}" alt="US DoE Model Integration" style="max-width: 90%; height: auto; display: inline-block; border-radius: 8px; border: 1px solid #eee;">
    <figcaption style="margin-top: 10px; color: #666;"><em>Integration architecture with the US DoE Simulink FCEV reference model.</em></figcaption>
</figure>

### Simulink Core Material Model
The core of the project involved building a high-fidelity Simulink model using **Hydralloy C2** to simulate real-world thermal loads and material response.

<figure style="text-align: center; margin: 0 auto 30px auto; display: block; width: 100%;">
    <img src="{{ '/hydc2_ovr.png' | relative_url }}" alt="Simulink Core Model" style="max-width: 90%; height: auto; display: inline-block; border-radius: 8px; border: 1px solid #eee;">
    <figcaption style="margin-top: 10px; color: #666;"><em>Simulink architecture featuring Hydralloy C2 material properties.</em></figcaption>
</figure>

### Reactor Control Granularity
To ensure efficient heat transfer, the internal control system of each individual reactor was modeled to manage pressure and temperature gradients during the hydride reaction.

<figure style="text-align: center; margin: 0 auto 30px auto; display: block; width: 100%;">
    <img src="{{ '/granul.png' | relative_url }}" alt="Reactor Control System" style="max-width: 75%; height: auto; display: inline-block; border-radius: 8px;">
    <figcaption style="margin-top: 10px; color: #666;"><em>Internal plan and control system for individual hydride reactors.</em></figcaption>
</figure>

---

## Experimental Validation

The following results compare our simulation data against experimental benchmarks for both the dehydration and hydration phases.

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 2%; margin: 20px 0; width: 100%;">
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/dehyd_plot.png' | relative_url }}" alt="Dehydration Plot" style="width: 100%; height: 280px; object-fit: contain; background: #fff; border-radius: 8px; border: 1px solid #eee;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Dehydration Performance vs. Experimental Data</em></p>
    </div>
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/hyd_plot.png' | relative_url }}" alt="Hydration Plot" style="width: 100%; height: 280px; object-fit: contain; background: #fff; border-radius: 8px; border: 1px solid #eee;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Hydration Performance vs. Experimental Data</em></p>
    </div>
</div>

---

## My Contributions

* Designed a novel open metal hydride cooling architecture integrated with the US DoE's FCEV reference model, leveraging metal hydride thermal properties to reduce auxiliary power consumption while maintaining effective thermal management.
* Developed automated material analysis tools in MATLAB to streamline property characterization across multiple metal hydride candidates, accelerating material selection and design iteration.
* Modeled isothermal pressure-composition behaviors in SIMULINK for various metal hydride materials, enabling accurate prediction of thermal performance and system optimization.
* Achieved an 18.8% reduction in AC load compared to conventional cooling systems, directly improving vehicle range and energy efficiency for hydrogen fuel cell electric vehicles.

## Technologies & Skills

* **Modeling & Simulation**: MATLAB, SIMULINK (Thermodynamic modeling, Heat transfer analysis)
* **Materials Engineering**: Metal hydride thermal properties, PCT curve analysis
* **Systems Integration**: US DoE FCEV reference model integration
* **Analysis**: Energy efficiency optimization, high-density heat transfer solutions

---

**Timeline**: January 2024 - May 2024