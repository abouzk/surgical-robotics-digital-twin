# Medical Robotics Digital Twin: Simulation & Haptics
**Context:** Mercer X Lab / Independent Research
**Status:** Architecture & Requirements Definition (Active Development)
**Timeline:** Jan 2026 – May 2026

## Project Overview
This project focuses on architecting a high-fidelity Digital Twin for **Surgical Robotics** using **Nvidia Isaac Sim** and **ROS 2 Humble**. The primary objective is to create a safe, simulated testbed for medical teleoperation, bridging the gap between theoretical kinematics and real-time control.

The development is split into two core phases:
1.  **Simulation Environment (Collaborative):** Developing a photorealistic surgery simulation scene to validate robot kinematics and collision physics.
2.  **Haptic Control & Safety (Independent):** Implementing a bilateral control loop with a **Phantom Omni** device, featuring **"Virtual Wall"** algorithms to enforce active safety constraints.

## System Architecture (Planned)
* **Simulation Engine:** Nvidia Isaac Sim
* **Middleware:** ROS 2 Humble (DDS Layer for real-time communication)
* **Hardware Interface:**
    * Input: Phantom Omni (Geomagic Touch) via OpenHaptics
    * Output: Simulated Medical Manipulator
* **Control Strategy:**
    * **Bilateral Teleoperation:** Force feedback functionality to convey tissue stiffness/collision to the operator.
    * **Virtual Fixtures (Virtual Walls):** Algorithms to define "Forbidden Zones" in the surgical workspace, mathematically constraining the tool tip to prevent damage to sensitive anatomy.

## Tech Stack
* **Languages:** Python, C++
* **Libraries:** Isaac Sim Core, ROS 2, OpenHaptics
* **Concepts:** Forward/Inverse Kinematics, Haptic Rendering, Active Constraints
