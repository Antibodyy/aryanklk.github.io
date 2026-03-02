---
title: "Two-Wheeled Balancing Robot using Model Predictive Control"
collection: projects
type: "Graduate Project"
permalink: /projects/balancing-robot
venue: "UC Berkeley"
location: "Berkeley, CA"
order: 5
---

Developed a high-performance self-balancing robotics system in the MuJoCo physics environment, implementing Model Predictive Control (MPC) for dynamic stabilization and trajectory tracking.

## System Architecture

The following flowchart illustrates the closed-loop interaction between the physical dynamics and the software control loop.

<figure style="text-align: center; margin: 0 auto 30px auto; display: block; width: 100%;">
    <img src="{{ '/overall_arch.png' | relative_url }}" alt="System Architecture" style="max-width: 85%; height: auto; display: inline-block; border-radius: 8px; border: 1px solid #eee;">
    <figcaption style="margin-top: 10px; color: #666;"><em>Figure 1: Overall hardware-software interaction architecture.</em></figcaption>
</figure>

---

## Simulation Performance

All simulations were conducted within the MuJoCo environment to validate the MPC controller's response to dynamic conditions.

### 1. Autonomous Start and Stop
The robot demonstrates smooth acceleration while maintaining vertical stability.

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 2%; margin: 20px 0; width: 100%;">
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/start_stop.gif' | relative_url }}" alt="Start Stop" style="width: 100%; height: 250px; object-fit: contain; background: #000; border-radius: 8px;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Autonomous Start/Stop Simulation</em></p>
    </div>
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/drive_stop_prediction_acc.png' | relative_url }}" alt="Accuracy" style="width: 100%; height: 250px; object-fit: contain; background: #fff; border-radius: 8px; border: 1px solid #eee;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Drive/Stop Prediction Accuracy</em></p>
    </div>
</div>

### 2. Perturbation Recovery
External forces were applied to test robustness; the system successfully returns to an upright position.

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 2%; margin: 20px 0; width: 100%;">
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/perturb_rec.gif' | relative_url }}" alt="Perturbation" style="width: 100%; height: 250px; object-fit: contain; background: #000; border-radius: 8px;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Perturbation Recovery Simulation</em></p>
    </div>
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/pitch_prediction_acc.png' | relative_url }}" alt="Pitch Performance" style="width: 100%; height: 250px; object-fit: contain; background: #fff; border-radius: 8px; border: 1px solid #eee;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Pitch Prediction Performance</em></p>
    </div>
</div>

### 3. Slope Balancing
The robot maintains its center of gravity when navigating inclined surfaces.

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 2%; margin: 20px 0; width: 100%;">
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/slope_bal.gif' | relative_url }}" alt="Slope Bal" style="width: 100%; height: 250px; object-fit: contain; background: #000; border-radius: 8px;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Slope Stability Simulation</em></p>
    </div>
    <div style="width: 49%; text-align: center;">
        <img src="{{ '/slope_stab_perf.png' | relative_url }}" alt="Slope Perf" style="width: 100%; height: 250px; object-fit: contain; background: #fff; border-radius: 8px; border: 1px solid #eee;">
        <p style="margin-top: 10px; font-size: 0.9em;"><em>Slope Stability Performance Graph</em></p>
    </div>
</div>

---

## My Contributions

* Designed and implemented a self-balancing robot using Model Predictive Control (MPC) algorithms for real-time dynamic stabilization.
* Integrated sensor fusion and state estimation to provide accurate feedback for the MPC controller, achieving stable performance under varying conditions.
* Executed complete hardware-software integration from sensor selection through control algorithm deployment in a simulated embedded robotics system.

## Technologies & Skills

* **Programming**: Python, C++, ROS2
* **Control Systems**: Model Predictive Control (MPC), State Estimation
* **Simulation**: MuJoCo
* **Robotics**: Sensor fusion, Embedded systems

---

**Timeline**: August 2025 - December 2025