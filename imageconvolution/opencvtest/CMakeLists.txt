cmake_minimum_required(VERSION 2.8)
project( opencvtest )
find_package( OpenCV REQUIRED )
set(-O3; -arch=compute_52)
add_executable( opencvgpu opencvgpu.cpp )
target_link_libraries( opencvgpu ${OpenCV_LIBS} )
