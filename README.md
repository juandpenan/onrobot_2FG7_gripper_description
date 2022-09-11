# Ros noetic description package for the onrobot 2fg7 gripper
------
## General info
This repository contains the URDF for the [onrobot 2fg7 gripper](https://onrobot.com/en/products/2fg7). It also has a simple control implementation to be used with gazebo simulator
this was developed using the [fusion 360 to urdf script](https://github.com/syuntoku14/fusion2urdf) and CAD files taken from the onrobot official webpage.
## Installation and ussage:
1. Install dependencies (from source):
  * [grasp fix gazebo plugin](https://github.com/JenniferBuehler/gazebo-pkgs/wiki/Installation)

  * [mimic joint fix plugin](https://github.com/roboticsgroup/roboticsgroup_upatras_gazebo_plugins) 
  
2. Install this package:
```
cd <your-catkin-ws>/src
git clone https://github.com/juandpenan/onrobot_2FG7_gripper_description
cd ..
catkin build onrobot_2fg7_description
```

3. Launch:

  * Display the gripper with RVIZ:
  ```
  roslaunch onrobot_2fg7_description display.launch
  ```
  
  * Launch gazebo: 
  ```
  roslaunch onrobot_2fg7_description gazebo_control.launch
  ```
