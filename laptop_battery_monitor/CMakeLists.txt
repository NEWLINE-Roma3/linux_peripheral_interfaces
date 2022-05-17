cmake_minimum_required(VERSION 3.0.2)
project(laptop_battery_monitor)

find_package(catkin REQUIRED COMPONENTS diagnostic_msgs sensor_msgs)

catkin_package(CATKIN_DEPENDS sensor_msgs diagnostic_msgs)

install(
  PROGRAMS 
    scripts/laptop_battery.py
    DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
