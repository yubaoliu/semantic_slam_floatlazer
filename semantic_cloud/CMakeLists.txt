cmake_minimum_required(VERSION 2.8)
project(floatlazer_semantic_cloud)

set(PACKAGE_DEPENDENCIES
  roscpp
	rospy
  sensor_msgs
)

find_package(catkin REQUIRED COMPONENTS ${PACKAGE_DEPENDENCIES})

include_directories(
  ${catkin_INCLUDE_DIRS}
)

# Make modules in include/ visible to work place
catkin_python_setup()

catkin_package(
  CATKIN_DEPENDS ${PACKAGE_DEPENDENCIES}
)
