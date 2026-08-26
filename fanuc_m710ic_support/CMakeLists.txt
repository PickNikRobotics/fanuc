cmake_minimum_required(VERSION 3.16)

project(fanuc_m710ic_support)

find_package(ament_cmake REQUIRED)

if (BUILD_TESTING)
  # find_package(roslaunch REQUIRED)
  # roslaunch_add_file_check(tests/roslaunch_test_m710ic45m.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_m710ic50.xml)
endif()

install(DIRECTORY config launch meshes urdf
  DESTINATION share/${PROJECT_NAME})

install(FILES readme.md DESTINATION share/${PROJECT_NAME})

ament_package()
