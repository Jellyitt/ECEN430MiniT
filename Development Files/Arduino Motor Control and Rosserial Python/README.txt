This system runs arduino 1.8.5
The code is a ROS node that communicates with the NUC through the rosserial_python node
This node subscribes to /cmd_vel and sends this for motor and speed control. While it publishes IMU data as geometry_msgs/Twist data type

How to run the arduino from terminal:
cd arduino-1.8.5/
./arduino

Note: Pressing tab on the keyboard autocompletes the word

File name:
Arduino Code - Motor Control - Bosch IMU -> Code using Bosch IMU
Arduino Code - Motor Control - MPU6050 IMU -> Code using MPU6050 IMU, used in the current system