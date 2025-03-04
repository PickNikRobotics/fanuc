cmake_minimum_required(VERSION 3.3)

project(fanuc_lrmate200id_support)

find_package(ament_cmake REQUIRED)

if (BUILD_TESTING)
  # find_package(roslaunch REQUIRED)
  # roslaunch_add_file_check(tests/roslaunch_test_200id.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_200id4s.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_200id4sc.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_200id4sh.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_200id7h.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_200id7l.xml)
  # roslaunch_add_file_check(tests/roslaunch_test_200id7lc.xml)
endif()

install(DIRECTORY config launch meshes urdf
  DESTINATION share/${PROJECT_NAME})

install(FILES readme.md DESTINATION share/${PROJECT_NAME})

ament_package()