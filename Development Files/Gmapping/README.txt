How to run gmapping in the current system set-up.

Ensure both laptop and NUC are connected to the modesttriangle network.

Firstly turn on the NUC:
roscore
NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch.launch

On the laptop:
ssh modesttrianglenuc@modesttrianglenuc-desktop
NT: cd catkin_ws/src/slam_gmapping/gmapping/launch
roslaunch <File name>
NT: rviz

Note: NT = open new terminal window
Note: min_launch.launch = launches rosserial python node (arduino), Lidar, Camera and static transforms

<File name>:
gmap_move.launch -> runs gmapping, map server CO249, move base
gmap2.launch -> runs gmapping, map server CO level two floor plan
gmap249.launch -> runs gmapping, map server CO249
gmapping.launch -> runs gmapping node
