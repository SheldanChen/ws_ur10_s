# Self-Collision Avoidance
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome#readme)


## Prerequisites
Build and test on Ubuntu 18.04.

## Installation

Please install [ros-melodic Desktop-Full Install](http://wiki.ros.org/melodic/Installation/Ubuntu) (since Gazebo is required as well),  [moveit! (Moveit! 1 melodic)](http://docs.ros.org/en/melodic/api/moveit_tutorials/html/index.html) in advance.  


## Building

Building workspace requires the following tools:

- Git (obviously)
- ROS Melodic (Desktop-Full Install)
- Gazebo (If you didn't install the Desktop-Full version ROS)
- Moveit! (Moveit! 1 for Melodic)

Get the source code:

```shell
git clone git@github.com:SheldanChen/ws_ur10_s.git
cd ws_ur10_s
```


To build everything, including the packages, /build file, /devel file, run in /ws_ur10_s:

```shell
catkin_make
```

Then source:

```shell
source ./devel/setup.bash
```


If you want to control the robot through a GUI, you can launch the simulation in RVIZ by:

```shell
roslaunch combination display.launch
```
to quit please input
```shell
Ctrl+c
```

If you want to control the robot through command lines, you can launch the simulation in Gazebo:
```shell
roslaunch combination gazebo.launch
```
and then open another terminal in /ws_ur10_s:
```shell
source ./devel/setup.bash
```


<!-- CONTACT -->
### Contact

Sheldan Chen - email@hkpc.org

Project Link: [https://github.com/SheldanChen/ws_ur10_s.git](https://github.com/SheldanChen/ws_ur10_s.git)

<p align="right">(<a href="#top">back to top</a>)</p>

