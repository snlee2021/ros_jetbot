# ros_jetbot

https://github.com/dusty-nv/jetbot_ros.git

Install ROS Melodic

Install Adafruit Libraries

Create catkin workspace

Build jetson-inference

Build ros_deep_learning

Build jetbot_ros

** darknet_ros.launch Source change : sudo gedit yoloobjectdetector.cpp
142 imagetransport_subscribe("/jetbot_camera/raw",~~

**순서대로 모두 설치

1. SWAP MEMORY 15G SET

 git clone https://github.com/JetsonHacksNano/resizeSwapMemory
 
 ./setSwapMemorySize -g 15

2. jetson nano power mode 5W SET

3. COMMAND

roscore

rosrun jetbot_ros jetbot_camera

roslaunch darknet_ros darknet_ros.launch

출처: https://taemian.tistory.com/entry/ROS-1-n-darknetros를-활용한-Yolo-v3-사용법 [Taemian]
