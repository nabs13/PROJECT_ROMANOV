# ROMANOV  -  Remotely cOntrolled MAppiNg lOcalization naVigation
Romanov is a mobile robot platform built from scratch, built as my familarity project with ROS systems.
The mobile plateform is meant to can be controlled remotely capable of SLAM - simulatenious Localization And Mapping.

## Components

- Rplider: https://www.amazon.com/Slamtec-RPLIDAR-Scanning-Avoidance-Navigation/dp/B07TJW5SXF/ref=sr_1_3?dchild=1&keywords=rplidar&qid=1631141923&sr=8-3
 
- 2 layer robot layer: https://www.amazon.com/wheel-layer-Chassis-Encoder-Arduino/dp/B06VTP8XBQ
 
- Motor driver L298N breakout board: https://www.amazon.com/DONGHENG-Controller-Module-Stepper-Arduino/dp/B07NMDQ4HC/ref=sr_1_22?dchild=1&keywords=rplidarL298N&qid=1631142019&sr=8-22

- Nvidia jetson nano: https://www.amazon.com/NVIDIA-Jetson-Nano-Developer-945-13541-0000-000/dp/B08J157LHH/ref=sr_1_3?crid=3SSJA8S8U39GM&dchild=1&keywords=nvidia+jetson+nano&qid=1631142222&sr=8-3
- Arduino uno: https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/ref=sr_1_3?dchild=1&keywords=arduino&qid=1631142273&sr=8-3

## Dependancies and Packages
- ROS on the jetson nano follow [this](https://www.stereolabs.com/blog/ros-and-nvidia-jetson-nano/) tutorial.
- 
- Install the arduino ide and install rosserial-arduino and upload the motor driver adruino code from [here](https://atadiat.com/en/e-rosserial-arduino-introduction/) make sure to either follow the same wiring pin configuration or you can edit the pin assignements to reflect what you have.

-Hector Slam package [here](https://github.com/NickL77/RPLidar_Hector_SLAM), be sure to configure the package as the tutorial requires. 

-Next is to install the teleop follow this tutuorial here

## Running packages 

- Run the following packages in different terminals each

- roscore //Run main ros core to get started

- rosrun rosserial_python serial_node.py /dev/ttyACM0 // connect ros to arduino board

- rosrun teleop_twist_keyboard teleop_twist_keyboard.py //load up keyboard control

- roslaunch rplidar_ros rplidar.launch //launch rpi lidar

- roslaunch hector_slam_launch tutorial.launch //launch hector mapping


## Todo 
- Install and integrate MPU 6050 hardware and drivers
- Develop TF2 relation broadcater and listener
- Add wheel encoders for odomtery   
