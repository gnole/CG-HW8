cmake_minimum_required(VERSION 3.15)

project(lab08)


set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenCV COMPONENTS core highgui REQUIRED)

add_executable(lab08 main.cpp )



target_include_directories(lab08
  PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/include
)

target_link_libraries(lab08
  PRIVATE opencv_core opencv_highgui
)
