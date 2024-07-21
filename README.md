# Udacity-Robotics-Project4
Udacity Robotics Software Engineer Nanodegree - Project 4: Map My World!

## Pre-requisite
1. RTAB-Map package is installed
```
sudo apt-get install ros-noetic-rtabmap
```

2. RTAB-Map ROS package is installed
```
sudo apt-get install ros-noetic-rtabmap-ros
```

## Build and Launch

1. Clone and initialize project with a catkin workspace
```
$ mkdir ~/catkin_ws && cd ~/catkin_ws
$ git clone https://github.com/izzianyramli/Udacity-Robotics-Project4.git
$ mv Udacity-Robotics-Project4 src
$ cd src && catkin_init_workspace
```

2. Go to `catkin_ws/` and build
```
$ cd ~/catkin_ws
$ catkin_make
```

3. Launch the robot world
```
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```

4. Open another terminal, and run robot teleop node
```
$ devel/setup.bash
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

5. Open another terminal, and launch the `RTAB-Map`
```
$ source devel/setup.bash
$ roslaunch my_robot mapping.launch
```
