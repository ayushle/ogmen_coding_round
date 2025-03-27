# 🤖 Bot Control Package

## 📌 Overview
The bot_description package defines the robot model using URDF/Xacro and provides launch files to visualize it in RViz, spawn it in an empty gazebo world and teleoperate it using keyboard.

## 📁 Directory Structure

'''
bot_description/
│── launch/          # Contains all launch files
    │── rviz.launch.py
    │── spawn.launch.py
    │── control.launch.py
│── description/     # URDF/Xacro files for robot description
    │── bot_structure.urdf.xacro
    │── gazebo_control.xacro
    │── inertial_macros.xacro
    │── sensor.xacro
│── config/          # Contains Rviz Config File
    │── bot.rviz
│── CMakeLists.txt   # CMake build configuration
│── package.xml      # Package metadata
'''


## 📁 Directory Structure

### **1️⃣ Visualizing the Robot in RViz
```bash    
        roslaunch bot_description rviz.launch.py
'''
### **12️⃣ Spawn Model in Gazebo World
```bash  
        roslaunch bot_description spawn.launch.py
'''
### **3️⃣ Control Model in Gazebo World
```bash  
        roslaunch bot_description control.launch.py
'''



