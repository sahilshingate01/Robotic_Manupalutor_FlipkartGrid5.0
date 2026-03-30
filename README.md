# 🤖 Robotic Manipulator - Flipkart GRiD 5.0

Developed by: **Sahil**

---

## 🌟 Overview

This repository contains the complete software stack and configuration for a **3-DOF (Degree of Freedom) Robotic Arm**, specifically designed and optimized for the **Flipkart GRiD 5.0** Robotics Challenge. The arm features a robust **Inverse Kinematics (IK)** solver, enabling precise positioning for pick-and-place operations based on real-time camera feedback.

## 🚀 Key Features

*   **3-DOF Planar Design**: Efficiently handles target objects within a defined workspace.
*   **Analytical Inverse Kinematics**: High-speed, precise target positioning.
*   **MoveIt! Integration**: Fully configured with the MoveIt Motion Planning Framework for advanced collision avoidance and trajectory planning.
*   **Vacuum Gripper Support**: Integrated logic for vacuum-based pick-and-place mechanisms.
*   **Vision-Ready**: Designed to interface with camera systems to receive target coordinates directly.
*   **Open-Loop & Closed-Loop Control**: Support for various motor control modes including direct angle control.

## 📁 Repository Structure

The codebase is organized into several modular ROS packages:

| Directory | Description |
| :--- | :--- |
| `3-DOF_Manipulator/` | Base manipulator configuration, including URDF and IKFast plugins. |
| `Final_working_with_vaccume/` | Finalized control scripts for the vacuum gripper assembly. |
| `SGP_robotic_arm/` | Primary MoveIt! configuration and launch files. |
| `robotic_arm_pkg/` | Core package containing essential nodes and message types. |
| `angle_ctrl/` | Specialized scripts for precise motor angle management. |
| `motor_test/` | Diagnostic tools for motor validation and calibration. |
| `ps4_comms/` | Support for manual control via PS4 controller. |
| `moveit_final_test/` | Validation suite for MoveIt motion plans. |

## 🛠️ Getting Started

### Prerequisites
*   **ROS** (Noetic/Melodic recommended)
*   **MoveIt!**
*   **OpenCV** (for vision-related features)
*   Standard Catkin build tools

### Installation
1.  Navigate to your catkin workspace `src` directory:
    ```bash
    cd ~/catkin_ws/src
    ```
2.  Clone this repository:
    ```bash
    git clone [repository_url]
    ```
3.  Build the workspace:
    ```bash
    cd ..
    catkin_make
    ```
4.  Source the workspace:
    ```bash
    source devel/setup.bash
    ```

### Launching the Simulation/Robot
To launch the main MoveIt demonstration:
```bash
roslaunch SGP_robotic_arm demo.launch
```

---

**Author**: [Sahil](mailto:sahilshingate0@gmail.com)  
**Project**: Robotic Manipulator - Flipkart GRiD 5.0
