# ARM Robotics

**A modular ROS 2 robotic manipulation system.**

ARM Robotics is a collection of interconnected ROS 2 packages developed to build a modular, intelligent robotic manipulation platform. The project focuses on robotic motion planning, control, perception, hardware integration, and vision-language-action (VLA) based manipulation.

The architecture separates individual capabilities into independent repositories, allowing each subsystem to be developed, tested, and integrated independently.

---

## System Architecture

The system is organized into five major subsystems:

### 1. Core & Motion Planning

| Repository | Description |
|---|---|
| [`arm_description`](https://github.com/IronMan1405/arm_description.git) | Robot description, URDF/Xacro models, and kinematic configuration. |
| [`arm_ik`](https://github.com/IronMan1405/arm_ik.git) | Inverse kinematics and Cartesian-to-joint-space computation. |
| [`arm_moveit_config`](https://github.com/IronMan1405/arm_moveit_config.git) | MoveIt 2 configuration for motion planning and execution. |

### 2. Control & Execution

| Repository | Description |
|---|---|
| [`arm_trajectory_executor`](https://github.com/IronMan1405/arm_trajectory_executor.git) | Executes joint-space and Cartesian motion trajectories. |
| [`arm_teleop`](https://github.com/IronMan1405/arm_teleop.git) | Teleoperation interface for controlling the robotic arm. |

### 3. Hardware & Safety

| Repository | Description |
|---|---|
| [`arm_driver`](https://github.com/IronMan1405/arm_driver.git) | Hardware interfaces, actuator communication, and low-level control. |
| [`arm_safety`](https://github.com/IronMan1405/arm_safety.git) | Safety mechanisms, operating limits, and emergency-stop functionality. |

### 4. Perception

| Repository | Description |
|---|---|
| [`arm_camera`](https://github.com/IronMan1405/arm_camera.git) | Camera integration, calibration, image publishing, and ArUco marker detection. |

### 5. Intelligence & Autonomous Manipulation

| Repository | Description |
|---|---|
| [`arm_vla`](https://github.com/IronMan1405/arm_vla.git) | Vision-Language-Action integration for language-conditioned robotic manipulation. |

---

## Technology Stack

- **Robotics Middleware:** ROS 2
- **Motion Planning:** MoveIt 2
- **Robot Description:** URDF / Xacro
- **Perception:** OpenCV, ArUco
- **VLA:** SmolVLA / LeRobot
- **Programming:** Python, C++

---

## Repository Structure

Each subsystem is maintained in its own repository under the `arm__` naming convention.

This modular approach enables independent development, testing, and maintenance while allowing the repositories to function together as a unified robotic system.

---

*An ongoing robotics engineering project.*