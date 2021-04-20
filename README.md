# yolo +  ros_jetbot

https://github.com/dusty-nv/jetbot_ros.git

Install ROS Melodic

Install Adafruit Libraries

Create catkin workspace

Build jetson-inference

Build ros_deep_learning

Build jetbot_ros

cd catkin_ws/src

git clone --recursive https://github.com/leggedrobotics/darknet_ros.git 

cd .. 



** darknet_ros.launch Source change : sudo gedit yoloobjectdetector.cpp
142 imagetransport_subscribe("/jetbot_camera/raw",~~

catkin_make -DCMAKE_BUILD_TYPE=Release 

빌드가 완료되었다면 

rospack profile



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

YOLO를 학습시키기

https://taehui.tistory.com/entry/YOLO-%EB%8D%B0%EC%9D%B4%ED%84%B0-%ED%95%99%EC%8A%B5-%EC%8B%9C%ED%82%A4%EA%B8%B0Weights-%ED%8C%8C%EC%9D%BC-%EB%A7%8C%EB%93%A4%EA%B8%B0
