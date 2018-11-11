How to run move_base in the current system set-up.

Ensure both laptop and NUC are connected to the modesttriangle network.

Firstly turn on the NUC:
roscore
NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch.launch

On the laptop:
ssh modesttrianglenuc@modesttrianglenuc-desktop
NT: cd catkin_ws/src/launch_file/launch
roslaunch <File name>
NT: rviz

Note: NT = open new terminal window
Note: min_launch.launch = launches rosserial python node (arduino), Lidar, Camera and static transforms

<File name>:
move_base.launch -> runs only move base node
move_base2.launch -> runs move base, map server, static transform
amcl_omni.launch -> runs move base, map server, static transform, amcl
all.launch -> runs move base, map server, static transform, amcl (old values in amcl)
