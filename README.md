***This is an ongoing project and not completed

# Autonomous 6-Wheeled Rover

This project aims to create an Autonomous 6-Wheeled Rover using ROS2 Humble. The rover is a rocker boogie type rover, and the design was taken from Thingiverse. The CAD model was then modified to fit the project's requirements. The main brains of the rover are a Raspberry Pi 4 running Ubuntu 22.04 server. The motors are DC motors with encoders, and they are controlled using a Pololu motor controller. Additionally, a Raspberry Pi Pico is used to interface with the motor controller and receive commands from ROS2 over USB.

![Design](/assets/fullstack2.png)

## Table of Contents
1. [Frame and URDF](#frame-and-urdf)
2. [Hardware](#hardware)
3. [Diff Plugin](#diff-plugin)
4. [ros2_control](#ros2_control)
5. [Gazebo](#gazebo)
6. [Launch Files](#launch-files)

## Frame and URDF
From the CAD model, STL meshes were created for each joint (not each CAD component). Using the CAD data, the center of mass and weight were estimated for the URDF file. Each wheel joint has been set, and RViz2 was used to visualize the frame.

### System Design
After market research of different available rovers, the "Martian Rover" design by Larkin Michael was chosen from Thingiverse. The chassis was 3D printed using PETG material. Modifications were made to accommodate additional electronics by creating plates inside the chassis for motor controllers and power distribution.

![Design](/assets/assembly/assembled1.png)

#### Modifying the CAD
The chassis model was exported to Fusion360 for modifications. Plates were added to the interior to house the motor controller and power distribution board. Additional plates were created to route wires from the interior to the exterior.

![CAD](/assets/CAD.png)

#### Assembly
The assembly process included steps such as mounting the power distribution board, soldering battery leads and wires for motor controllers, creating a custom motor controller and encoder prototype board, extending motor wires, installing motors, and testing encoder outputs.

![Assembly](/assets/assembly/motor_driver9.png)
![Assembly3](/assets/assembly/motor_wire3.png)

## Hardware
The rover's main components include a Raspberry Pi 4 running Ubuntu 22.04 server, DC motors with encoders, and a Pololu motor controller. The Raspberry Pi Pico is used to control the motors, receiving commands from ROS2 over USB.

![Assembly2](/assets/assembly/first_floor.png)

## Diff Plugin
This project includes a fork of a repository initially made for Arduino. The original code has been heavily modified to work with the Raspberry Pi Pico, while still using the same commands from ROS2 nodes for communication.

## ros2_control


## Gazebo


## Launch Files
| Launch File       | Description                            |
|-------------------|----------------------------------------|
| rsp.launch        | Launches the Robot State Publisher.    |
| launch_sim        | Launches the simulation mode.          |
| launch_rover      | Launches the rover mode.               |


