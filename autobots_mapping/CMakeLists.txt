cmake_minimum_required(VERSION 2.8.3)
project(autobots_mapping)

add_compile_options(-std=c++14)

find_package(catkin REQUIRED COMPONENTS roscpp roslaunch)

roslaunch_add_file_check(launch)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES autobots_mapping
#  CATKIN_DEPENDS other_catkin_pkg
#  DEPENDS system_lib
)

include_directories(
include
${catkin_INCLUDE_DIRS}
)
