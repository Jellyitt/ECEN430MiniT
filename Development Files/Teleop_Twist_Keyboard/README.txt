How to run teleop_twist_keyboard in the current system set-up.

Ensure both laptop and NUC are connected to the modesttriangle network.

Firstly turn on the NUC:
roscore
NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch.launch

On the laptop:
ssh modesttrianglenuc@modesttrianglenuc-desktop
NT: rosrun teleop_twist_keyboard teleop_twist_keyboard.py
NT: rviz

Note: NT = open new terminal window