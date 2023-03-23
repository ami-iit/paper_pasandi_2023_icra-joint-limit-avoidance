<h1 align="center">
Torque Control with Joints Position and Velocity Limits Avoidance
</h1>

<div align="center">

V. Pasandi, D. Pucci, "Torque Control with Joints Position and Velocity Limits Avoidance" in IEEE 2023 International Conference on Robotics and Automation (ICRA)

</div>

Video

<p align="center">

<div align="center">
2023 International Conference on Robotics and Automation (ICRA)
</div>

<div align="center">
  <a href="Paper"><b>Paper</b></a> |
  <a href="Pre=print"><b>Pre-print</b></a> |
  <a href="Video"><b>Video</b></a>
</div>

## Abstract
The design of a control architecture for providing the desired motion along with the realization of the joint limitation of a robotic system is still an open challenge in control and robotics.
This paper presents a torque control architecture for fully actuated manipulators for tracking the desired time-varying trajectory while ensuring the joints position and velocity limits.
The presented architecture stems from the parametrization of the feasible joints position and velocity space by exogenous states.
The proposed parametrization transforms the control problem with constrained states to an un-constrained one by replacing the joints position and velocity with the exogenous states.
With the help of Lyapunov-based arguments, we prove that the proposed control architecture ensures the stability and convergence of the desired joint trajectory along with the joints position and velocity limits avoidance.
We validate the performance of proposed architecture through various simulations on a simple two-degree-of-freedom manipulator and the humanoid robot iCub.

## Dependencies
This repository depends upon the following Softwares:

  - [MATLAB/Simulink](https://fr.mathworks.com/products/matlab.html), default version R2018b,

And specifically for [two link manipulator simulation](software/twoLinkManipulator):

  - [MATLAB/Simscape](https://fr.mathworks.com/products/simscape.html), default version R2018b,

And specifically for [humanoid robot iCub simulation](software/humanoidRobotIcub):

  - [Gazebo Simulator](https://gazebosim.org/home), default version 11.12.0,
  - [WB-Toolbox](https://github.com/robotology/WB-Toolbox), [gazebo-yarp-plugins](https://github.com/robotology/gazebo-yarp-plugins), [icub-models](https://github.com/robotology/icub-models) and [YARP](https://github.com/robotology/yarp)

## Installation and Usage
The repository is tested and developed on Ubuntu operating system.
Some functionalities may not work properly on macOS and Windows.

  - Install the required dependencies,
    
    It is suggested to install WB-Toolbox, gazebo-yarp-plugins, icub-models and YARP and their dependencies using [robotology-superbuild](https://github.com/robotology/robotology-superbuild) (Note that in this case one needs to enable ROBOTOLOGY_ENABLE_DYNAMICS, ROBOTOLOGY_USES_GAZEBO and ROBOTOLOGY_USES_MATLAB options).

  - Clone the repository on your pc by running on a terminal
  
  ```
  git clone https://github.com/ami-iit/paper_pasandi_2023_icra-joint-limit-avoidance
  ```
  or download the repository.

  - Simply use the available functionalities. For the step-by-step guideline, please refer to [software readme](software/README.md).

## Citing this work
If you find the work useful, please consider citing:

```bibtex
@INPROCEEDINGS{00000,
  author={{Pasandi, Venus and Pucci, Daniele},
  booktitle={2023 International Conference on Robotics and Automation (ICRA)}, 
  title={Torque Control with Joints Position and Velocity Limits Avoidance}, 
  year={2023},
  volume={},
  number={},
  pages={0-0},
  doi={00000}}
```

### Maintainer

This repository is maintained by:

| | |
|:---:|:---:|
| [<img src="https://github.com/VenusPasandi.png" width="80">](https://github.com/VenusPasandi) | [@VenusPasandi](https://github.com/VenusPasandi) |
