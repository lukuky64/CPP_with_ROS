cmake_minimum_required(VERSION 3.0.2)
project(ros_interact)

# Find catkin and any catkin packages
find_package(catkin REQUIRED COMPONENTS roscpp std_msgs)

# Declare a catkin package
catkin_package()

# Specify additional locations of header files
include_directories(include ${catkin_INCLUDE_DIRS})

# Add executable
add_executable(${PROJECT_NAME}_node src/ros_interact.cpp)

# Add dependencies
add_dependencies(${PROJECT_NAME}_node ${${PROJECT_NAME}_EXPORTED_TARGETS} ${catkin_EXPORTED_TARGETS})

# Link libraries
target_link_libraries(${PROJECT_NAME}_node ${catkin_LIBRARIES})
