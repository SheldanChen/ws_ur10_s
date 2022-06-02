# Self-Collision Avoidance

[![Build Status](https://jenkins.platform.dev.nuxeo.com/buildStatus/icon?job=nuxeo/nuxeo/master)](https://jenkins.platform.dev.nuxeo.com/job/nuxeo/job/nuxeo/job/master/)

Tested/Build on UBUNTU 18.04.

## Installation

Please install [ros-melodic Desktop-Full Install (since Gazebo is required as well)](http://wiki.ros.org/melodic/Installation/Ubuntu),  [moveit! (Moveit! 1 melodic)](http://docs.ros.org/en/melodic/api/moveit_tutorials/html/index.html) in advance.  


## Building

Building workspace requires the following tools:

- Git (obviously)
- ROS Melodic (Desktop-Full Install)
- Gazebo (If you didn't install the Desktop-Full version ROS)
- Moveit! (Moveit! 1 for Melodic)

Get the source code:

```shell
git clone git@github.com:SheldanChen/test_sheldan.git
cd test_sheldan
```


To build everything, including the packages, /build file, /devel file, run in /test_sheldan:

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
and then open another terminal in /test_sheldan:
```shell
source ./devel/setup.bash
```



### Reporting Issues

You can follow the developments in the [Nuxeo Platform](https://jira.nuxeo.com/browse/NXP/) project of our JIRA bug tracker.

You can report issues on [answers.nuxeo.com](http://answers.nuxeo.com).

## Licensing

