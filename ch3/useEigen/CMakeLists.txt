cmake_minimum_required(VERSION 3.5)
project(useEigen)

set(CMAKE_BUILD_TYPE "Release")
set(CMAKE_CXX_FLAGS "-O3")

# Find Eigen3
find_package(Eigen3 3.3 REQUIRED)

# Include Eigen3 directories
include_directories(${EIGEN3_INCLUDE_DIRS})

# Add executable
add_executable(eigenMatrix eigenMatrix.cpp)