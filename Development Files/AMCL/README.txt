How to run AMCL in the current system set-up.

Ensure both laptop and NUC are connected to the modesttriangle network.

Firstly turn on the NUC:
roscore
NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch.launch

On the laptop:
ssh modesttrianglenuc@modesttrianglenuc-desktop
NT: cd catkin_ws/src/launch_file/launch
roslaunch amcl_omni2.launch

Note: NT = open new terminal window

File name:
amcl_omni2.launch -> runs map_server and AMCL nodes
amcl_omni.launch -> runs map_server, AMCL, move base and a static transform