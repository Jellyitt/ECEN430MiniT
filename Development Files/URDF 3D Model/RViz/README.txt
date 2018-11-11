How to run URDF model for RViz in the current system set-up.

Ensure both laptop and NUC are connected to the modesttriangle network.

Firstly turn on the NUC:
roscore
NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch.launch

On the laptop:
ssh modesttrianglenuc@modesttrianglenuc-desktop
NT: cd catkin_ws/src/simpleModel
rosrun simpleModel urdf_visualize.launch model:='$(find simpleModel)/urdf/simpleModel.urdf'

Note: NT = open new terminal window
Note: min_launch.launch = launches rosserial python node (arduino), Lidar, Camera and static transforms