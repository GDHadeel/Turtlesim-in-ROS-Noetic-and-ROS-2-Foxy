# Turtlesim-in-ROS-Noetic-and-ROS-2-Foxy

## Description 
This repository provides a simple guide to manipulate the Turtlesim package in both ROS Noetic and ROS 2 Foxy to draw basic shapes: a circle and a square. The Turtlesim package is a beginner-friendly tool that helps new ROS users learn basic ROS concepts by visualizing the movements of a simulated turtle.

---

* Start by opening a terminal using Ctrl + Alt + T.

### Manipulate with turtlesim package in ROS noetic

1. Open a terminal and start roscore:
     ```bash
     roscore
     ```
     
2. Open another terminal and install the turtlesim package:
     ```bash
     sudo apt-get install ros-noetic-turtlesim
     ```
     
3. Run the turtlesim node:
     ```bash
     rosrun turtlesim turtlesim_node
     ```
4. Draw a Circle:
   - Open another terminal and run the following command to control the turtle and draw a circle:
     ```bash
     rosrun turtlesim turtle_teleop_key
     ```
     
5. output:
  <img width="452" alt="image" src="https://github.com/GDHadeel/Turtlesim-in-ROS-Noetic-and-ROS-2-Foxy/assets/126657301/a1740d80-bb19-4bd8-b0c5-bc8a9524ff86">

---

### Manipulate with turtlesim package in ROS2 foxy

1. Open a terminal and source the ROS 2 setup script
     ```bash
     source /opt/ros/foxy/setup.bash
     ```
     
2. Install the turtlesim package:
     ```bash
     sudo apt-get install ros-foxy-turtlesim
     ```
     
3. Run the turtlesim node:
     ```bash
     ros2 run turtlesim turtlesim_node
     ```
4. Draw a Square:
   - Open another terminal, source the ROS 2 setup script again
     ```bash
     source /opt/ros/foxy/setup.bash
     ```
   - Move forward:
     ```bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.0}}" -1
     sleep 2
     ```
   - Turn 90 degrees:
     ```bash
     source /opt/ros/foxy/setup.bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.5708}}" -1
     sleep 1
     ```
   - Move forward:
     ```bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.0}}" -1
     sleep 2
     ```
   - Turn 90 degrees:
     ```bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.5708}}" -1
     sleep 1
     ```
     - Move forward:
     ```bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.0}}" -1
     sleep 2
     ```
   - Turn 90 degrees:
     ```bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.5708}}" -1
     sleep 1
     ```
   - Move forward:
     ```bash
     ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.0}}" -1
     sleep 2
     ```
     
5. output:
  <img width="434" alt="image" src="https://github.com/GDHadeel/Turtlesim-in-ROS-Noetic-and-ROS-2-Foxy/assets/126657301/992beca9-7246-41a7-970c-0db019d9b5b3">

---

## Acknowledgements
https://wiki.ros.org/turtlesim




