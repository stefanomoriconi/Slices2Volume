cmake_minimum_required(VERSION 2.8)
 
project(Slices2Volume)
 
find_package(ITK REQUIRED)
include(${ITK_USE_FILE})
if (ITKVtkGlue_LOADED)
  find_package(VTK REQUIRED)
  include(${VTK_USE_FILE})
endif()
 
add_executable(Slices2Volume Slices2Volume.cpp)
 
target_link_libraries(Slices2Volume ${ITK_LIBRARIES})