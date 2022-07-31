cmake_minimum_required(VERSION 3.0.0)

project(keyauth CXX)

add_library(keyauth INTERFACE)

target_include_directories(keyauth INTERFACE 
  inc/
)

target_link_libraries(keyauth INTERFACE
  ${CMAKE_CURRENT_LIST_DIR}/lib/library_x86.lib
  ${CMAKE_CURRENT_LIST_DIR}/lib/libcurl.lib
)