cmake_minimum_required(VERSION 3.5.0)

project(decadarobotics_devtest)

#===============================================================================

find_package(catkin QUIET)

if (catkin_FOUND)

  catkin_package()

  install(
    DIRECTORY launch
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
  )

else()
  message("catkin not found so skipping this ROS1 package")
endif()
