cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
#project(pcl-test_pcl)
project(correspondence_grouping)

find_package(PCL 1.7.2 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (correspondence_grouping correspondence_grouping.cpp)
target_link_libraries (correspondence_grouping ${PCL_LIBRARIES})
#add_executable (test_pcl test_pcl.cpp)
#target_link_libraries (test_pcl ${PCL_LIBRARIES})
#project(pcd_write)

#add_executable (pcd_write pcd_write.cpp)
#add_executable (pcl_test pcl_test.cpp)
#target_link_libraries (pcd_write ${PCL_LIBRARIES})
#target_link_libraries (pcl_test ${PCL_LIBRARIES})
