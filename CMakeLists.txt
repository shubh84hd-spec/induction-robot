cmake_minimum_required(VERSION 3.8)
project(simple_robot_description)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY assets launch
  DESTINATION share/${PROJECT_NAME}
)
install(
  FILES robot.urdf
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
