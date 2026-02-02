# Isaac Sim Digital Twin: RPI Mercer X Lab
**Status:** Architecture & Requirements Definition (Active Development)
**Timeline:** Jan 2026 – May 2026

## Project Overview
This project focuses on architecting a high-fidelity Digital Twin for the RPI Mercer X Lab using **Nvidia Isaac Sim** and **ROS 2 Humble**. The goal is to create a bilateral control loop that couples physical haptic devices (Phantom Omni) with a simulated industrial environment for teleoperation training.

## System Architecture (Planned)
* **Simulation Engine:** Nvidia Isaac Sim
* **Middleware:** ROS 2 Humble (DDS Layer for real-time communication)
* **Hardware Interface:**
    * Input: Phantom Omni Haptic Device
* **Control Strategy:**
    * Bilateral Teleoperation with force feedback.
    * Virtual Fixtures for collision avoidance and operator guidance.

## Tech Stack
* **Languages:** Python, C++
* **Libraries:** Isaac Sim Core, ROS 2, OpenHaptics
