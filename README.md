Notification
====================

This work is unofficial, unsupported and in progress in the current location.

Description
====================
This repository contains RViz and Gazebo simulations of the da Vinci Surgical System controlled using ROS. 

# Author

Ankur Agrawal:asagrawal@wpi.edu

Radian Azhar Gondokaryono:ragondokaryono@wpi.edu


# Install
* download & compile dvrk_env

```sh
# cd to catkin ws src dir
cd /PATH/TO/CATKIN_WS/src
# clone repo
git clone https://github.com/WPI-AIM/dvrk_env.git
# build
cd ..
catkin_make
```
# Packages

This is a short description of the packages in this repository. The detailed explanations and instructions are available in the packages itself.

dvrk_gazebo: Provides launch files to launch PSM, MTM, ECM, SUJ Cart and the full dvrk models in gazebo.

dvrk_gazebo_control: Provides example codes to control the gazebo simulation.

dvrk_model: Provides CAD models, URDFs, SDFs of PSM, ECM, MTM, Laprotek Master and the SUJ Cart. Additionally it has launch files for all of the models in RViz. **Copy and Paste the Folders: Cart, dvrk, ECM, MTM, and PSM to ~/.gazebo/models**

dvrk_plugins: Has the model plugin which provides interface between the dvrk simulation in Gazebo and ROS.

laprotek_comm: Provides interface between Laprotek and ROS.

# Launching 
```sh
# Run the Surgical System simulation
roslaunch dvrk_gazebo dvrk_gazebo.launch
```
# Dependencies

Gazebo 7, ROS kinetic or ROS indigo, gazebo_ros_pkgs. If ROS-indigo is to be used with Gazebo 7, keep gazebo_ros_pkgs (https://github.com/ros-simulation/gazebo_ros_pkgs/tree/indigo-devel) in your src folder.
