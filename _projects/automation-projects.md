---
title: "Two-Wheeled Balancing Robot (MPC Control)"
collection: projects
type: "Graduate Project"
permalink: /projects/balancing-robot
venue: "UC Berkeley"
location: "Berkeley, CA"
order: 5
---

Developed a high-performance self-balancing robotics system in the MuJoCo physics environment, implementing Model Predictive Control (MPC) for dynamic stabilization and trajectory tracking.

## System Architecture

The following flowchart illustrates the closed-loop interaction between the physical dynamics (MuJoCo) and the software control architecture.

<figure class="project-figure" style="text-align: center; margin: 0 auto 20px auto; display: block;">
    <img src="{{ '/overall_arch.png' | relative_url }}" alt="Overall Architecture" style="display: block; margin: 0 auto; max-width: 100%;">
    <figcaption style="text-align: center; margin-top: 8px;"><em>Physical and Software Interaction Architecture</em></figcaption>
</figure>

## Simulation Performance

All simulations were conducted within the MuJoCo environment to validate the MPC controller's response to dynamic environments.

### Autonomous Start and Stop
The robot demonstrates smooth acceleration and deceleration while maintaining vertical stability. The graph shows the high correlation between predicted velocity and actual performance.

<div style="display: flex; justify-content: center; gap: 20px; text-align: center; margin: 20px 0;">
    <figure class="project-figure" style="margin: 0; flex: 1;">
        <img src="{{ '/start_stop.gif' | relative_url }}" alt="Start Stop Simulation" style="max-width: 100%; height: auto;">
        <figcaption style="margin-top: 8px;"><em>Autonomous Start/Stop</em></figcaption>
    </figure>
    <figure class="project-figure" style="margin: 0; flex: 1;">
        <img src="{{ '/drive_stop_prediction_acc.png' | relative_url }}" alt="Drive Stop Accuracy" style="max-width: 100%; height: auto;">
        <figcaption style="margin-top: 8px;"><em>Drive/Stop Prediction Accuracy</em></figcaption>
    </figure>
</div>

### Perturbation Recovery
To test robustness, external forces were applied to the robot. The system successfully estimates state deviation and applies corrective torque to return to an upright position.

<div style="display: flex; justify-content: center; gap: 20px; text-align: center; margin: 20px 0;">
    <figure class="project-figure" style="margin: 0; flex: 1;">
        <img src="{{ '/perturb_rec.gif' | relative_url }}" alt="Perturbation Recovery" style="max-width: 100%; height: auto;">
        <figcaption style="margin-top: 8px;"><em>Perturbation Recovery</em></figcaption>
    </figure>
    <figure class="project-figure" style="margin: 0; flex: 1;">
        <img src="{{ '/pitch_prediction_acc.png' | relative_url }}" alt="Pitch Prediction Accuracy" style="max-width: 100%; height: auto;">
        <figcaption style="margin-top: 8px;"><em>Pitch Prediction Performance</em></figcaption>
    </figure>
</div>

### Slope Balancing
The robot maintains its center of gravity even when navigating inclined surfaces, showcasing the adaptability of the sensor fusion and state estimation algorithms.

<div style="display: flex; justify-content: center; gap: 20px; text-align: center; margin: 20px 0;">
    <figure class="project-figure" style="margin: 0; flex: 1;">
        <img src="{{ '/slope_bal.gif' | relative_url }}" alt="Slope Balancing" style="max-width: 100%; height: auto;">
        <figcaption style="margin-top: 8px;"><em>Slope Stability Simulation</em></figcaption>
    </figure>
    <figure class="project-figure" style="margin: 0; flex: 1;">
        <img src="{{ '/slope_stab_perf.png' | relative_url }}" alt="Slope Stability Performance" style="max-width: 100%; height: auto;">
        <figcaption style="margin-top: 8px;"><em>Slope Stability Performance Graph</em></figcaption>
    </figure>
</div>

---

## My Contributions

* Designed and implemented a self-balancing robot using Model Predictive Control (MPC) algorithms for real-time dynamic stabilization.
* Integrated sensor fusion and state estimation to provide accurate feedback for the MPC controller, achieving stable performance under varying conditions.
* Executed complete hardware-software integration from sensor selection through control algorithm deployment in a simulated embedded robotics system.

## Technologies & Skills

* **Programming**: Python, C++, ROS2
* **Control Systems**: Model Predictive Control (MPC), Real-time State Estimation
* **Simulation**: MuJoCo Physics Engine
* **Robotics**: Sensor fusion, Embedded systems, Hardware-software integration

---

**Timeline**: August 2025 - December 2025