# Integrated Mobile Evaluation Testbed for Robotics Operations (iMETRO)
iMETRO is a facility designed to catalyze the adaptation of advanced terrestrial robotic technologies for space exploration use cases, such as logistics, maintenance, and science utilization within environments designed for human exploration on the Lunar and Martian surfaces. The iMETRO focus is on Intra-Vehicular Activity (IVA) environments, such as surface habitats, pressurized rover cabins, and space station internal modules. The iMETRO goal is to increase the availability of end-to-end systems enabling remote operation of robots in space supervised by humans on Earth. These systems include ground control user interfaces and software for managing robot remote control with realistic latency, bandwidth, and coverage interruptions for various mission environments (e.g., Low Earth Orbit, cis-Lunar, Lunar Surface, Mars Surface).

> **_NOTE:_**  The core content of this repository is in the process of being released through NASA's release process. This should be available very soon.

## iMETRO Software
 
* The software includes 
  * Open-source robot configurations (e.g., URDF) for iMETRO robots.
  * MoveIt2 interfaces to the robots for interacting from an application layer.
  * ros2_control controllers for controlling the various joints of the robots.
  * Models of mock-ups for space use cases, such as the crew access hatch and logistics stowage task trainer.
  * ros2_control hardware interfaces for interacting with the actuatl hardware (not used in sim)
 
## Pysical Facility Features
 
* Mockups of space use cases as described above
* Physical robots with software interfaces (see below for more info)
* Frame-mounted PTZ cameras
* Remote operator stations for situational awareness
* Isolated robot network with configurable latency and bandwidth restrictions (currently a future planned capability)
 
## Available Robots
### Linear rail-mounted single manipulator (available now)
* Universal Robots UR10e
* Robotiq hand-E Gripper w/ Custom Fingers
* Vention horizontally mounted 2.0m linear rail
* Ewellix Telescoping Lift Kit with 700mm Stroke
* Intel® RealSense™ Wrist-Mounted Depth Camera
 
### Mobile Base Dual Manipulator (in development)
* Universal Robots UR5e (2x)
* Robotiq Hand-E Grippers with Custom Fingers
* Arms mounted to dual, independent lift-kits of 500mm Stroke
* Clearpath Ridgeback Wheeled Mobile Base
* Intel® RealSense™ Wrist-Mounted Depth Cameras
 
### Bring your own components!
* Integrate your own sensors and/or end effectors into our hardware system utilizing standard ROS interfaces
* Bring your own entire robot to interact with the other space application mockups
 
### Documentation
* See [here](https://ntrs.nasa.gov/api/citations/20240013956/downloads/iMETRO%20Year%202%20Poster.pdf) for an early poster of the work.
* See [here](https://ntrs.nasa.gov/citations/20240007666) for a video utilizing the facility to perform a maintenance demonstration
* A paper describing the facility published at the [Ubiquitous Robots](https://2025.ubiquitousrobots.org/) conference will be available soon