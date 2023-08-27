### Steps to creating a cpp package to interact with ros

#### Compile using Cmake
##### rom VSCode:
```ruby
cd build
cmake .
make
```

##### From ubuntu terminal:
```ruby
~/catkin_ws
catkin_make
```

### Run from ubuntu terminal:
```ruby
~/catkin_ws/src/robotics_studio_2023/build/devel/lib/ros_interact/ros_interact_node
```


```ruby
source /opt/ros/noetic/setup.bash
cd ~/catkin_ws/src
catkin_create_pkg your_package_name std_msgs roscpp
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```
