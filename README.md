# Autonomous 6-Wheeled Rover

This project aims to create an Autonomous 6-Wheeled Rover using ROS2 Humble. The rover is a rocker boogie type rover, and the design was taken from Thingiverse. The CAD model was then modified to fit the project's requirements. The main brains of the rover are a Raspberry Pi 4 running Ubuntu 22.04 server. The motors are DC motors with encoders, and they are controlled using a Pololu motor controller. Additionally, a Raspberry Pi Pico is used to interface with the motor controller and receive commands from ROS2 over USB.

## Table of Contents
1. [Hardware](#hardware)
2. [Diff Plugin](#diff-plugin)
3. [Frame and URDF](#frame-and-urdf)
4. [ros2_control](#ros2_control)
5. [Gazebo](#gazebo)
6. [Launch Files](#launch-files)

## Hardware
The rover's main components include a Raspberry Pi 4 running Ubuntu 22.04 server, DC motors with encoders, and a Pololu motor controller. The Raspberry Pi Pico is used to control the motors, receiving commands from ROS2 over USB.

## Diff Plugin
This project includes a fork of a repository initially made for Arduino. The original code has been heavily modified to work with the Raspberry Pi Pico, while still using the same commands from ROS2 nodes for communication.

## Frame and URDF
From the CAD model, STL meshes were created for each joint (not each CAD component). Using the CAD data, the center of mass and weight were estimated for the URDF file. Each wheel joint has been set, and RViz2 was used to visualize the frame.

## ros2_control


## Gazebo


## Launch Files
| Launch File       | Description                            |
|-------------------|----------------------------------------|
| rsp.launch        | Launches the Robot State Publisher.    |
| launch_sim        | Launches the simulation mode.          |
| launch_rover      | Launches the rover mode.               |


