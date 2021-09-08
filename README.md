# ROMANOV  -  Remotely cOntrolled MAppiNg lOcalization naVigation
Romanov is a mobile robotic platform built from scratch, mostly using components readily available in Ghana.
The mobile plateform is meant to can be controlled remotely capable of SLAM - simulatenious Localization And Mapping.

## Components
- Rplider: https://www.amazon.com/Slamtec-RPLIDAR-Scanning-Avoidance-Navigation/dp/B07TJW5SXF/ref=sr_1_3?dchild=1&keywords=rplidar&qid=1631141923&sr=8-3
- 2 layer robot layer: https://www.amazon.com/wheel-layer-Chassis-Encoder-Arduino/dp/B06VTP8XBQ
- Motor driver L298N breakout board: https://www.amazon.com/DONGHENG-Controller-Module-Stepper-Arduino/dp/B07NMDQ4HC/ref=sr_1_22?dchild=1&keywords=rplidarL298N&qid=1631142019&sr=8-22
- Nvidia jetson nano: https://www.amazon.com/NVIDIA-Jetson-Nano-Developer-945-13541-0000-000/dp/B08J157LHH/ref=sr_1_3?crid=3SSJA8S8U39GM&dchild=1&keywords=nvidia+jetson+nano&qid=1631142222&sr=8-3
- Arduino uno: https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/ref=sr_1_3?dchild=1&keywords=arduino&qid=1631142273&sr=8-3

## Dependancies and Packages
- Install and have ROS running on the jetson nano follow [this](https://www.stereolabs.com/blog/ros-and-nvidia-jetson-nano/) tutorial.
- Install the arduino ide and install rosserial-arduino and upload the motor driver adruino code from [here](https://atadiat.com/en/e-rosserial-arduino-introduction/) make sure to either follow the same wiring pin configuration or you can edit the pin assignements to reflect what you have.
- Next is to install the teleop `sudo apt-get install ros-melodic-teleop-twist-keyboard`

## Runing packages 


## Todo 
