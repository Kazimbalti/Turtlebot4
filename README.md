# nav2_minimal_turtlebot_simulation

A minimum description & simulation of the TB3/TB4 using standard ROS-GZ tools for ``nav2_bringup`` and user example.

It is largely ROS distribution agnostic, using launch files and URDFs so it should be easy to use for any ROS 2 distribution & release into Rolling for all future ones. 

### **1. Installation**
```
1. mkdir -p ~/turtlebot4_ws/src
2. cd ~/turtlebot4_ws/src
3. Clone this repository in your src as
   git clone https://github.com/Kazimbalti/Turtlebot4.git
4. cd ..
5. colcon build
6. source install/setup.bash
```


### **2. Implementation** 

```
Launch turtlebot4 gazebo simulator, rviz and teleop control
```
    In terminal 1:
    cd ~/turtlebot4_ws
    source install/setup.bash
    ros2 launch nav2_minimal_tb4_sim simulation.launch.py
```
Then teleop the turtlebot4 using
```
    In terminal 1:
    cd ~/turtlebot4_ws
    source install/setup.bash
    sudo apt update
    sudo apt install ros-humble-teleop-twist-keyboard
    ros2 run teleop_twist_keyboard teleop_twist_keyboard

```

#### Thanks to Steve Macenski and ClearPath Robotics

