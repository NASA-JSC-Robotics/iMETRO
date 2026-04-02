![imetro ](resources/imetro_full_border.png)

# iMETRO: Integrated Mobile Evaluation Testbed for Robotics Operations

iMETRO is a robotics facility housed at NASA's Johnson Space Center with the goal of adapting advanced terrestrial robotic technologies for space exploration applications such as logistics, maintenance, and science utilization tasks.
These applications are designed for human exploration environments on space stations or the Lunar and Martian surfaces.
The high fidelity mockups, test beds, and end-to-end systems provided can be used to develop capabilities that enable remote operation of robots in space supervised by humans on Earth.
Particular focus is given to Intra-Vehicular Activity (IVA) environments of surface habitats, pressurized rover cabins, and space station internal modules.

Some of these systems include ground control user interfaces and software for managing robot remote control with realistic latency, bandwidth, and coverage interruptions for various mission environments (e.g., Low Earth Orbit, cis-Lunar, Lunar Surface, Mars Surface).

> **_NOTE:_** The core content referenced in this repository is in the process of being released through NASA's release process.
> Additional packages will be released as noted below.

## Software Features

The iMETRO facility includes robot software for:

- Open-source robot configurations (e.g., URDF, deploy files) for iMETRO robots
- ros2_control controllers for controlling the various joints of the robots
- Basic MoveIt2 configurations for robots for interfacing with the systems from an application layer
- Models of mock-ups for space use cases, such as the crew access hatch and logistics stowage task trainer
- ros2_control hardware interfaces for interacting with the physical hardware (not used in sim)

## Physical Facility Features

- Mockups of space use cases as described above
- Physical robots with software interfaces (see below for more info)
- Frame-mounted PTZ cameras
- Remote operator stations for situational awareness
- Isolated robot network with configurable latency and bandwidth restrictions (currently a future planned capability)

## Available Robots

### Linear rail-mounted single manipulator

- Universal Robots UR10e
- Robotiq hand-E Gripper with Custom Fingers
- Vention horizontally mounted 2.0m linear rail
- Ewellix Telescoping Lift Kit with 700mm Stroke
- Intel® RealSense™ Wrist-Mounted Depth Camera

The primary description and deployment package are available in [chonkur_l_raile](https://github.com/NASA-JSC-Robotics/chonkur_l_raile).

We also include the base containerized workflow for deploying the controllers on hardware, a kinematic simulation, and a dynamic simulation in [clr_ws](https://github.com/NASA-JSC-Robotics/clr_ws).

Included in that workspace is a basic pick and place demonstration using the dynamic simulation, for more information refer to the [clr_sim_demos](https://github.com/NASA-JSC-Robotics/clr_sim_demos) project.

A video of this demonstration in simulation is shown below.

https://github.com/user-attachments/assets/604accbe-7c7c-43f0-9e32-9c1a6ff31a09

### Mobile Base Dual Manipulator

- Universal Robots UR5e (2x)
- Robotiq Hand-E Grippers w/ Custom Fingers
- Arms mounted to dual, independent lift-kits of 500mm Stroke
- Clearpath Ridgeback Wheeled Mobile Base
- Intel® RealSense™ Wrist-Mounted Depth Cameras

Base description, package, and deployment files can be found in [phoebe_bridgeback](https://github.com/NASA-JSC-Robotics/phoebe_bridgeback), and a pick and place of a cylinder in simulation is shown below.

[phoebe_cylinder_demo_mujoco_smaller.webm](https://github.com/user-attachments/assets/5b7163dc-ec6b-4832-981f-6030eacea077)

Like CLR, a containerized workflow for deploying the robot on hardware, a kinematic simulation, and a full dynamic simulartion are available in [phoebe_bridgeback_ws](https://github.com/NASA-JSC-Robotics/phoebe_bridgeback_ws).

### Bring Your Own

- Integrate your own sensors and/or end effectors into our hardware system utilizing standard ROS interfaces
- Bring your own entire robot to interact with the other space application mockups

### Documentation

- See [our paper published at the Ubiquitous Robotics Conference](https://ieeexplore.ieee.org/document/11077983) for a detailed explanation of the facility with an outline of a representative use case
- See [the iMETRO poster](https://ntrs.nasa.gov/api/citations/20240013956/downloads/iMETRO%20Year%202%20Poster.pdf) for an early poster of the work
- See [our video](https://ntrs.nasa.gov/citations/20240007666) of utilizing the facility to perform a maintenance demonstration
- See [our International Conference on Robotics and Automation (ICRA) paper](https://ntrs.nasa.gov/citations/20260001395) for information about our MuJoCo simulation and sim-to-real transfer efforts

### Citation

If you use this software in your own work, please cite the following paper:

```bibtex
@INPROCEEDINGS{imetro-facility-2025,
  author={Dunkelberger, Nathan and Sheetz, Emily and Rainen, Connor and Graf, Jodi and Hart, Nikki and Zemler, Emma and Azimi, Shaun},
  booktitle={2025 22nd International Conference on Ubiquitous Robots (UR)},
  title={Design of the iMETRO Facility: A Platform for Intravehicular Space Robotics Research},
  year={2025},
  volume={},
  number={},
  pages={390-397},
  keywords={NASA;Moon;Seals;Maintenance engineering;Maintenance;Robots;Standards;Open source software;Testing;Logistics},
  doi={10.1109/UR65550.2025.11077983}}
```

If you use the dynamic simulation software in your own work, please cite the following paper:
```bibtex
@INPROCEEDINGS{imetro-sim-2026,
  author={Hart, Nikki and Dunkelberger, Nathan and Holum, Erik and Kavraki, Lydia E. and Zemler, Emma and Azimi, Shaun},
  booktitle={NASA Technical Reports Server},
  title={The iMETRO Dynamic Simulation: An Open-Source Simulator for Intravehicular Space Robotics Research},
  year={2026},
  note={Accepted for publication at the International Conference of Robotics and Automation.},
  url={https://ntrs.nasa.gov/citations/20260001395}}
```

### Contact Information

Questions are best asked through issues.

For more information [**Connect With Us HERE**](https://www.nasa.gov/reference/jsc-robotics/).
