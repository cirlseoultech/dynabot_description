# Dynabot Robot Description (URDF)
## Overview

This package contains a simplified robot description (URDF) of the [Dynabot](https://www.youtube.com/channel/UCvLNY4Xos34DEHYCKBYXAZA) developed by [Control and Intelligent Robotic Lab](https://sites.google.com/site/cdslweb), Seoultech.

The extended Dynabot description, simulation, and control software is available exclusively to members of the [Control and Intelligent Robotic Lab](https://sites.google.com/site/cdslweb). For more information and membership applications, contact jungsu@seoultech.ac.kr.

**Author & Maintainer: Jung-Su Kim, [Control and Intelligent Robotic Lab]**

![alt text](https://github.com/cirlseoultech/dynabot_description/blob/main/picture/robot.jpg?raw=true)

## Usage

Load the Dynabot description to the ROS parameter server:

    roslaunch dynabot_description load.launch

To visualize and debug the robot description, start the standalone visualization (note that you have to provide the following additional dependencies: `joint_state_publisher`, `robot_state_publisher`, `rviz`):

    roslaunch dynabot_description standalone.launch

### Launch files

* **`load.launch`:** Loads the URDF to the parameter server. Meant to be included in higher level launch files.

* **`standalone.launch`:** A standalone launch file that starts RViz and a joint state publisher to debug the description.
