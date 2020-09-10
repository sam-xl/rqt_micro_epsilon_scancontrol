cmake_minimum_required(VERSION 2.8.3)
project(rqt_micro_epsilon_scancontrol)

find_package(catkin REQUIRED)

catkin_package()
catkin_python_setup()

install(PROGRAMS 
  scripts/rqt_micro_epsilon_scancontrol
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)

install(DIRECTORY 
  resource
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(FILES 
  plugin.xml
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)