# jnmouse_description

ROS package with URDF description macro for [Jetson Nano Mouse](https://rt-net.jp/products/jetson_nano_mouse/)

![](https://rt-net.github.io/images/jetson-nano-mouse/jnmouse_rviz.png)

## Requirements

- ROS
  - [Melodic Morenia](http://wiki.ros.org/melodic/Installation/Ubuntu)

## Installation

```sh
# Clone jnmouse_description and install dependencies
cd ~/catkin_ws/src
git clone https://github.com/rt-net/jnmouse_description
rosdep install -r -y -i --from-paths .

# Build the package
cd ~/catkin_ws
catkin build
source devel/setup.bash
```

## How to Use

Display the robot model of Jetson Nano Mouse on RViz with the following comand.

```sh
roslaunch jnmouse_description display_xacro.launch 
```

## LICENSE

(C) 2020 RT Corporation \<support@rt-net.jp\>

This repository is licensed under the Apache License, Version 2.0, see [LICENSE](./LICENSE).  
Unless attributed otherwise, everything in this repository is under the Apache License, Version 2.0.


### Acknowledgements

Special thanks to https://gbiggs.github.io/rosjp_urdf_tutorial_text/index.html