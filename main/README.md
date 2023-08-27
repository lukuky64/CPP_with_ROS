### Steps to creating a cpp package to interact with ros
```ruby
source /opt/ros/noetic/setup.bash
cd ~/catkin_ws/src
catkin_create_pkg your_package_name std_msgs roscpp
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```
