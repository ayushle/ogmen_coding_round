# 🤖 Bot Control Package

## 📌 Overview

The `bot_control` package is responsible for controlling the robot using ROS 2. It includes nodes for processing sensor data and sending control commands.

## 📁 Directory Structure

```
bot_control/
│── description/     # URDF/Xacro files for robot description
    │── bot_structure.urdf.xacro
    │── gazebo_control.xacro
    │── inertial_macros.xacro
    │── sensor.xacro
│── launch/          # Contains launch files
    │── rviz.launch.py
│── scripts/          # scripts
    │── reading_laser.cpp  #This ROS 2 node filters LiDAR scan data, limiting the field of view to 120° and publishing the refined data for navigation or obstacle avoidance.
│── CMakeLists.txt   # CMake build configuration
│── package.xml      # Package metadata
│── README.md        # Documentation

```


## 🏗️ Usage

### **1️⃣ Running the Control Node**
To run a control node:
```bash
ros2 run bot_control rviz.launch.py
```
