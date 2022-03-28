slam_gmapping [![Build Status](https://travis-ci.com/ros-perception/slam_gmapping.svg?branch=melodic-devel)](https://travis-ci.org/ros-perception/slam_gmapping)
================================================================================================================================================================

* [gmapping (ROS Wiki)](https://wiki.ros.org/gmapping)

---


# Build

```sh
mkdir ws_2dslam/src
git clone <xxx>
cd ..
catkin_make -j4
```

# Run

```sh
rosbag play --clock <bag-file>

rosparam set use_sim_time true
rosrun gmapping slam_gmapping scan:=base_scan
# or
roslaunch gmapping slam_gmapping_pr2.launch
```

rosgraph

<p align="center">
  <img src="./imgs/rosgraph.png" style="width:80%;">
</p>

rviz

<p>
  <img src="./imgs/rviz.png" style="width:100%;">
</p>