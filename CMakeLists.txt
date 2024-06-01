cmake_minimum_required(VERSION 3.10)
project(exfat_sum)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# disable building of shared libraries
set(BUILD_SHARED_LIBS OFF)

# add the -static flag
set(CMAKE_EXE_LINKER_FLAGS "-static")

# add the executable
add_executable(exfat_sum exfat_sum.cpp)