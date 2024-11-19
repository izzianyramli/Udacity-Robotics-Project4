# Udacity-Robotics-Project4
Udacity Robotics Software Engineer Nanodegree - Project 4: Map My World!


## Build and Launch

1. Clone repo and build workspace
```bash
$ mkdir ~/catkin_ws && cd ~/catkin_ws
$ git clone https://github.com/izzianyramli/Udacity-Robotics-Project4.git src
$ catkin_make
```

2. Launch robot world
```bash
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```

3. Launch teleop keyboard
```bash
$ source devel/setup.bash
$ roslaunch teleop_twist_keyboard teleop_twist_keyboard.py
```

4. Launch SLAM
```bash
$ source devel/setup.bash
$ roslaunch my_robot mapping.launch
```

5. Once finished mapping, run RTABMap Viewer
```bash
$ rtabmap-databaseViewer ~/.ros/rtabmap.db
```
