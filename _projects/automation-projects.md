---
title: "Two-Wheeled Balancing Robot (MPC Control)"
collection: projects
type: "Graduate Project"
permalink: /projects/balancing-robot
venue: "UC Berkeley"
location: "Berkeley, CA"
order: 5
---

Developed a high-performance self-balancing robotics system in the MuJoCo physics environment, implementing Model Predictive Control (MPC) for dynamic stabilization and trajectory tracking. This project highlights the intersection of advanced control theory and embedded systems integration.

## System Architecture

The interaction between the physical dynamics (simulated in MuJoCo) and the software control loop is visualized below:

<div style="text-align: center; margin-bottom: 20px;">
  <img src="/images/overall_arch.png" alt="System Architecture Flowchart" style="width: 80%; display: block; margin: 0 auto;">
  <p><i>Figure 1: Overall hardware-software interaction architecture.</i></p>
</div>

---

## Performance & Simulation Results

### 1. Autonomous Start and Stop
The robot demonstrates smooth acceleration and deceleration while maintaining vertical stability. The accompanying graph shows the high correlation between predicted velocity and actual performance.

<div style="display: flex; justify-content: center; align-items: center; gap: 10px; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="/images/start_stop.gif" alt="Start/Stop Simulation" style="width: 100%; border-radius: 8px;">
  </div>
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="/images/drive_stop_prediction_acc.png" alt="Drive/Stop Accuracy Graph" style="width: 100%; border-radius: 8px;">
  </div>
</div>

### 2. Perturbation Recovery
To test the robustness of the MPC controller, external forces were applied to the robot. The system successfully estimates the state deviation and applies corrective torque to return to an upright position.

<div style="display: flex; justify-content: center; align-items: center; gap: 10px; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="/images/perturb_rec.gif" alt="Perturbation Recovery" style="width: 100%; border-radius: 8px;">
  </div>
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="/images/pitch_prediction_acc.png" alt="Pitch Prediction Accuracy" style="width: 100%; border-radius: 8px;">
  </div>
</div>

### 3. Slope Balancing
The robot is capable of maintaining its center of gravity even when navigating inclined surfaces, showcasing the adaptability of the sensor fusion and state estimation algorithms.

<div style="display: flex; justify-content: center; align-items: center; gap: 10px; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="/images/slope_bal.gif" alt="Slope Balancing" style="width: 100%; border-radius: 8px;">
  </div>
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="/images/slope_stab_perf.png" alt="Slope Stability Performance" style="width: 100%; border-radius: 8px;">
  </div>
</div>

---

## Technical Contributions

* **MPC Implementation**: Designed and implemented a self-balancing algorithm using Model Predictive Control for real-time stabilization.
* **Sensor Fusion**: Integrated state estimation to provide accurate feedback for the MPC controller, ensuring stability under varying conditions.
* **MuJoCo Simulation**: Executed complete hardware-software logic within a high-fidelity physics engine before deployment considerations.

## Technologies & Skills

* **Programming**: Python, C++, ROS2
* **Control Systems**: Model Predictive Control (MPC), State Estimation
* **Physics Engines**: MuJoCo
* **Robotics**: Sensor fusion, embedded systems, hardware-software integration

**Timeline**: August 2025 - December 2025