***This is an ongoing project and not completed

# Autonomous 6-Wheeled Rover

This project aims to create an Autonomous 6-Wheeled Rover using ROS2 Humble. The rover is a rocker boogie type rover, and the design was taken from Thingiverse. The CAD model was then modified to fit the project's requirements. The main brains of the rover are a Raspberry Pi 4 running Ubuntu 22.04 server. The motors are DC motors with encoders, and they are controlled using a Pololu motor controller. Additionally, a Raspberry Pi Pico is used to interface with the motor controller and receive commands from ROS2 over USB.

![Design](/assets/fullstack2.png)

# Wiki
The documentation of the build process can be found at the Wiki Section or [Here](https://github.com/shivammehta220/rover_bot/wiki/Home/)

# Launch Files

| Launch File       | Description                            |
|-------------------|----------------------------------------|
| rsp.launch        | Launches the Robot State Publisher.    |
| launch_sim        | Launches the simulation mode.          |
| launch_rover      | Launches the rover mode.               |


