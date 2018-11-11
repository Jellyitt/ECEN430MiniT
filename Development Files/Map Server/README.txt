How to run map_server in the current system set-up.

Ensure both laptop and NUC are connected to the modesttriangle network.

Firstly turn on the NUC:
roscore
{ NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch.launch }

On the laptop:
ssh modesttrianglenuc@modesttrianglenuc-desktop
NT: cd catkin_ws/src/launch_file/launch
roslaunch map_server.launch
NT: rviz

Note: NT = open new terminal window
      {} = optional

File name:
min_launch.launch = launches rosserial python node (arduino), Lidar, Camera and static transforms