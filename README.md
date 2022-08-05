# turtlebot3-SLAM-map

create and save a map using turtlebot3 with SLAM approach

1- satrt with installing ROS dependacies, type the following command in terminal 

$ sudo apt-get install ros-noetic-joy ros-noetic-teleop-twist-joy \
  ros-noetic-teleop-twist-keyboard ros-noetic-laser-proc \
  ros-noetic-rgbd-launch ros-noetic-rosserial-arduino \
  ros-noetic-rosserial-python ros-noetic-rosserial-client \
  ros-noetic-rosserial-msgs ros-noetic-amcl ros-noetic-map-server \
  ros-noetic-move-base ros-noetic-urdf ros-noetic-xacro \
  ros-noetic-compressed-image-transport ros-noetic-rqt* ros-noetic-rviz \
  ros-noetic-gmapping ros-noetic-navigation ros-noetic-interactive-markers
  
  
  2- type the following commands to install turtlebot3
  $ sudo apt install ros-noetic-dynamixel-sdk
  $ sudo apt install ros-noetic-turtlebot3-msgs
  $ sudo apt install ros-noetic-turtlebot3
  
  
  3- type the following commands to install simulation packages 
  $ cd ~/catkin_ws/src/
  $ git clone -b noetic-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
  $ cd ~/catkin_ws && catkin_make
  
  4- launch the navigation 
  $ export TURTLEBOT3_MODEL=burger
  $ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
  
  ![image](https://user-images.githubusercontent.com/79508459/183106245-0681d6b5-bdfb-41b5-bc1f-654eac29c5ac.png)

  
  5- launch simulation world
  $ export TURTLEBOT3_MODEL=burger
  $ roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch
  
  ![image](https://user-images.githubusercontent.com/79508459/183106284-b46d6a8b-553f-40a8-aa2e-e193b8fa4619.png)

  
  
  $ export TURTLEBOT3_MODEL=waffle 
  $ roslaunch turtlebot3_gazebo turtlebot3_world.launch
  
 ![image](https://user-images.githubusercontent.com/79508459/183106313-ce71306c-ecd4-4df2-a29f-8deed5824635.png)
 
  
  
  
