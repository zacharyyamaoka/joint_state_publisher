cmake_minimum_required(VERSION 3.5)
project(joint_state_publisher_gui_local)

find_package(ament_cmake REQUIRED)

# Install the urdf folder
# install(DIRECTORY launch config urdf
#   DESTINATION share/${PROJECT_NAME}
# )

# Install the executable for joint_state_publisher_gui.py
install(
  PROGRAMS joint_state_publisher_gui_local/joint_state_publisher_gui.py
  DESTINATION lib/${PROJECT_NAME}
)

# Install the Python package as-is
ament_python_install_package(${PROJECT_NAME})

ament_package()