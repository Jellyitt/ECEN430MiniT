How to run fiducials in the current system set-up.
On the NUC currently:

Without launch files:
roscore
NT: roslaunch realsense_camera r200_nodelet_default.launch
NT: rosrun aruco_detect aruco_detect camera:=/camera/color/image_raw camera_info:=/camera/color/camera_info
NT: roslaunch fiducial_slam fiducial_slam.launch
NT: roslaunch fiducial_slam fiducial_rviz.launch


With launch files:
roscore
NT: cd catkin_ws/src/launch_file/launch
roslaunch min_launch2.launch

Note: NT = New Terminal