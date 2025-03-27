
# 🌍 Bot World Package

## 📌 Overview

The `bot_world` package is responsible for **defining the simulation environment** for the robot. It includes world files for **Gazebo simulation** and launch files to load the world and spawn the robot inside it.

## 📁 Directory Structure

```  
bot_world/
│── launch/          # Contains launch files
│   ├── spawn.launch.py  # Spawns the robot inside the world
│── worlds/          # Gazebo world files
│   ├── world1.world  # Custom world definition
│── description/     # URDF/Xacro files for robot description
    │── bot_structure.urdf.xacro
    │── inertial_macros.xacro
│── CMakeLists.txt   # CMake build configuration
│── package.xml      # Package metadata
│── README.md        # Documentation
```  



## 🏗️ Usage

### **1️⃣ Launching the Gazebo World**
To launch the simulation environment in Gazebo and spawn bot in that:
```  bash
        ros2 launch bot_world spawn.launch.py
```  
