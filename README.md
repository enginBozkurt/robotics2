# Robotics Book Draft

Copyright (c) Frank Dellaert and Seth Hutchinson, All rights Reserved

The code in the notebooks and python .py files is covered by the BSD license, like GTSAM; see the LICENSE.BSD file for details.

The remainder (including all markdown cells in the notebooks and other prose) is not licensed for any redistribution or change of format or medium, other than making copies of the notebooks or forking this repo for your own private use. No commercial or broadcast use is allowed. We are making these materials freely available to help you learn robotics, so please respect our copyright and these restrictions.


One python notebook per section.

Current Draft TOC:

## Discrete: Trash Sorter (https://www.amprobotics.com/)
- State:		plastic|paper|cardboard|metal|glass|unknown
- Actuators: 	gripper (4 actions or no-op)
- Sensors: 	Attributes -> colors (5), size (SML), weights (LH)
- Perception: 	Estimation probabilities of plastic|paper|cardboard|metal|unknown
- Planning: 	Decision Theory -> sort into three bins (plastics|mixed paper|metals|glass) or do nothing


## Discrete: Vacuum Cleaner
- State:		house
- Actuators: 	noisy graph
- Sensors: 	noisy light
- Perception: 	HMM
- Planning: 	MDP

## 2D: Logistics Platform
- State:		x,y
- Actuators: 	swedish wheels, round robot
- Sensors: 	2D LIDAR
- Perception: 	Localization
- Planning: 	Graph-based stuff, config space

## x,y,theta: Duckiebot
- State:		x, y, theta (not fully SE(2) and 3x3 matrices yet)
- Actuators: 	differential drive
- Sensors: 	Camera, image formation
- Perception: 	CNN Place Recognition
- Planning: 	Dubbins etc

## SE(2): Autonomous Vehicle
- State:		SE(2): SO(2) and 3x3 homogeneous
- Actuators: 	Ackerman steering
- Sensors: 	3D LIDAR
- Perception: 	ICP, Pose-SLAM
- Planning: 	Motion Primitives

## SE(3): Drone
- State:		SE(3): SO(3) and 4x4 homogeneous
- Actuators: 	Quad-rotor
- Sensors: 	Camera in 3D, geometry, stereo
- Perception: 	Visual SLAM
- Planning: 	Trajectory Optimization

## Learning
- Discrete - 2D - SE(2) - SE(2) in 3D - SE(3)
- Machine Learning - RL - Deep learning - DRL
